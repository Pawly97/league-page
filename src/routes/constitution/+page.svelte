<script>
    import { dues } from '$lib/utils/helper';
    let one, oneOne, oneOneOne, oneTwo, oneTwoOne, oneTwoTwo, oneTwoThree, oneTwoFour, oneTwoFive, oneThree;
    let two, twoOne, twoTwo, twoThree;
    let three, threeOne;
    let four, fourOne, fourTwo;
    let five, fiveOne;
    let six, sixOne, sixTwo, sixThree;
    let seven, sevenOne, sevenTwo, sevenThree;

    const goToSection = (section) => {
        const top = section.getBoundingClientRect().top + window.pageYOffset;
        window.scrollTo({left: 0, top, behavior: 'smooth'});
    }
</script>

<style>
    .constitution {
        position: relative;
        z-index: 1;
        width: 92%;
        max-width: 800px;
        margin: 8em auto 10em;
    }

    h1 {
        font-size: 2em;
        line-height: 1.2em;
        text-align: center;
        margin: 2em 0 1.5em;
    }

    h2 {
        font-size: 1.5em;
        line-height: 1.2em;
    }

    h3 {
        text-decoration: underline;
        font-size: 1.3em;
        line-height: 1.2em;
    }

    h4 {
        text-decoration: underline;
        margin-left: 2em;
        font-size: 1.2em;
        line-height: 1.2em;
    }

    h5 {
        margin-left: 6em;
        font-size: 0.8em;
        line-height: 1.1em;
    }

    .subBlock {
        margin-left: 2.4em;
    }

    .sectionHeading {
        margin: 4em 0 1.5em;
    }

    .subSectionHeading {
        margin: 1.5em 0 1.5em;
    }

    .underscore {
        text-decoration: underline;
    }

    .right {
        text-align: right;
    }

    .positionMaximums td {
        min-width: 3em;
    }

    .noUnderscore {
        text-decoration: none;
    }

    .clickable {
        cursor: pointer;
    }

    .clickable:hover {
        color: #00316b;
    }

    p {
        color: #777;
    }
</style>

<div class="constitution">
    <h1 class="noUnderscore">LEGENDS LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
<h3 class="noUnderscore clickable" onclick={() => goToSection(one)}>Section 1: League Format</h3>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(oneOne)}>1.1 Teams and Draft</h4>

<h3 class="noUnderscore clickable" onclick={() => goToSection(two)}>Section 2: Roster Composition</h3>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(twoOne)}>2.1 Starting Lineup and Reserves</h4>

<h3 class="noUnderscore clickable" onclick={() => goToSection(three)}>Section 3: Taxi Squad Rules</h3>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(threeOne)}>3.1 Taxi Squad Management</h4>

<h3 class="noUnderscore clickable" onclick={() => goToSection(four)}>Section 4: Scoring System</h3>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(fourOne)}>4.1 Passing</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(fourTwo)}>4.2 Rushing</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(fourThree)}>4.3 Receiving</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(fourFour)}>4.4 Kicking</h4>

<h3 class="noUnderscore clickable" onclick={() => goToSection(five)}>Section 5: Other Rules</h3>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveOne)}>5.1 Trades</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveTwo)}>5.2 Waivers</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveThree)}>5.3 Playoffs</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(fiveFour)}>5.4 Tanking Policy and Draft Order</h4>

<h3 class="noUnderscore clickable" onclick={() => goToSection(six)}>Section 6: Trading</h3>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(sixOne)}>6.1 Trade Collusion</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(sixTwo)}>6.2 Lending Players Prohibition</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(sixThree)}>6.3 Veto/Trade Process</h4>

<h3 class="noUnderscore clickable" onclick={() => goToSection(seven)}>Section 7: Replacing Managers</h3>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenOne)}>7.1 Removing Managers</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenTwo)}>7.2 Replacing Managers</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(sevenThree)}>7.3 Replacement Incentive</h4>

<h3 class="noUnderscore clickable" onclick={() => goToSection(eight)}>Section 8: League Finances</h3>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(eightOne)}>8.1 League Dues</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(eightTwo)}>8.2 Payout</h4>
    <h4 class="noUnderscore clickable" onclick={() => goToSection(eightThree)}>8.3 Raising Dues</h4>

<hr />

<!-- Section 1: League Format -->
<h2 class="sectionHeading" bind:content={this.one}>Section 1: League Format</h2>

<h3 class="subSectionHeading" bind:content={this.oneOne}>1.1 Teams and Draft</h3>
<p>League Size: 12 teams</p>
<ul>
  <li>Draft Type: Snake draft</li>
  <li>Rookie Draft: 4-round rookie draft each year</li>
  <li>Keeper League: Keep most players year to year; manage rosters through drafts, trades, and waivers</li>
</ul>

<!-- Section 2: Roster Composition -->
<h2 class="sectionHeading" bind:content={this.two}>Section 2: Roster Composition</h2>

<h3 class="subSectionHeading" bind:content={this.twoOne}>2.1 Starting Lineup and Reserves</h3>
<p class="underscore">Starting Lineup</p>
<ul>
  <li>1 QB</li>
  <li>2 WR</li>
  <li>2 RB</li>
  <li>1 TE</li>
  <li>3 Flex (WR, RB, TE)</li>
</ul>
<p>Bench: 6 spots</p>
<p>IR: 3 spots (players must be designated as IR, Out, or similar in the Sleeper App)</p>
<p>Taxi Squad: 3 spots</p>

<!-- Section 3: Taxi Squad Rules -->
<h2 class="sectionHeading" bind:content={this.three}>Section 3: Taxi Squad Rules</h2>

<h3 class="subSectionHeading" bind:content={this.threeOne}>3.1 Taxi Squad Management</h3>
<ul>
  <li>Pre-Season Setup: Place up to 4 players on Taxi Squad</li>
  <li>In-Season: No new additions to Taxi Squad. Players can be moved to the active roster but cannot return to the Taxi Squad</li>
</ul>

<!-- Section 4: Scoring System -->
<h2 class="sectionHeading" bind:content={this.four}>Section 4: Scoring System</h2>

<h3 class="subSectionHeading" bind:content={this.fourOne}>4.1 Passing</h3>
<div class="subBlock">
  <ul>
    <li>1 point per 25 yards (0.04 per yard)</li>
    <li>4 points per passing TD</li>
    <li>2 points for 2-point conversion</li>
    <li>-1 point per interception</li>
    <li>1 point for 40+ yard completion bonus</li>
    <li>1 point for 40+ yard pass TD bonus</li>
    <li>1 point for 50+ yard pass TD bonus</li>
  </ul>
</div>

<h3 class="subSectionHeading" bind:content={this.fourTwo}>4.2 Rushing</h3>
<div class="subBlock">
  <ul>
    <li>1 point per 10 yards (0.10 per yard)</li>
    <li>6 points per rushing TD</li>
    <li>2 points for 2-point conversion</li>
    <li>1 point for 40+ yard rush bonus</li>
    <li>1 point for 40+ yard rush TD bonus</li>
    <li>1 point for 50+ yard rush TD bonus</li>
  </ul>
</div>

<h3 class="subSectionHeading" bind:content={this.fourThree}>4.3 Receiving</h3>
<div class="subBlock">
  <ul>
    <li>0.5 points per reception</li>
    <li>1 point per 10 yards (0.10 per yard)</li>
    <li>6 points per receiving TD</li>
    <li>2 points for 2-point conversion</li>
    <li>1 point for 40+ yard reception bonus</li>
    <li>1 point for 40+ yard reception TD bonus</li>
    <li>1 point for 50+ yard reception TD bonus</li>
  </ul>
</div>

<h3 class="subSectionHeading" bind:content={this.fourFour}>4.4 Kicking</h3>
<div class="subBlock">
  <ul>
    <li>FG Made (0-39 yards): 3 points</li>
    <li>FG Made (40-49 yards): 4 points</li>
    <li>FG Made (50+ yards): 5 points</li>
    <li>PAT Made: 1 point</li>
  </ul>
</div>

<!-- Section 5: Other Rules -->
<h2 class="sectionHeading" bind:content={this.five}>Section 5: Other Rules</h2>

<h3 class="subSectionHeading" bind:content={this.fiveOne}>5.1 Trades</h3>
<p>Trades are allowed anytime, with a trade deadline in week 13. Tradable assets include players, draft picks, and FAAB $. Pending trades are subject to a 2-day review period.</p>

<h3 class="subSectionHeading" bind:content={this.fiveTwo}>5.2 Waivers</h3>
<div class="subBlock">
  <p>FAAB Bidding system with a $100 budget per team and a $0 minimum bid. Players are locked upon the start of their week’s game and remain on waivers for 2 days after being dropped. Waivers clear on Wednesdays at 1 AM MDT. Custom daily waivers are allowed, with players locking at game start.</p>
</div>

<h3 class="subSectionHeading" bind:content={this.fiveThree}>5.3 Playoffs</h3>
<div class="subBlock">
  <p>Playoffs start in Week 14 with 8 teams qualifying based on regular season standings. Each playoff round lasts one week, using default seeding (teams remain on their initial bracket side). Non-playoff teams compete in a Toilet Bowl bracket, where losers advance to determine the last-place team (“💩 King”).</p>
</div>

<h3 class="subSectionHeading" bind:content={this.fiveFour}>5.4 Tanking Policy and Draft Order</h3>
<div class="subBlock">
  <p>Bottom 4 teams (based on regular season standings) enter a lottery to determine draft order. Lottery entries are assigned as follows:</p>
  <ul>
    <li>12th place: 4 entries</li>
    <li>11th place: 3 entries</li>
    <li>10th place: 2 entries</li>
    <li>9th place: 1 entry</li>
  </ul>
  <p>Teams caught purposely tanking, as voted on by the league, will forfeit their 1st round draft pick(s) and be subject to a $100 fine.</p>
  <p>Draft order for playoff teams is determined by playoff placement, with regular season standings as the tiebreaker. For example, among teams losing in the semi-finals, the team with the lower regular season standing gets the higher pick.</p>
</div>

<!-- Section 6: Trading -->
<h2 class="sectionHeading" bind:content={this.six}>Section 6: Trading</h2>

<h3 class="subSectionHeading" bind:content={this.sixOne}>6.1 Trade Collusion</h3>
<div class="subBlock">
  <p>If any owners are suspected of accepting/offering bribes to enhance their/another owner’s team via trade, trading assets other than fantasy players, draft picks, or FAAB $, or otherwise found guilty of collusion*, all parties involved will face punishment:</p>
  <ul>
    <li>First Offense: Immediate reduction of FAAB budget by 80%</li>
    <li>Second Offense: Immediate freeze on all transactions for the next 18 weeks of regular season and playoff games, including trades and waiver bids</li>
    <li>Third Offense: League meeting of uninvolved members to discuss next steps</li>
  </ul>
  <p>All collusive trades will be reversed/denied. If a trade affected prior game outcomes, results will be revised.</p>
  <p>*Collusion includes organizing veto votes against acceptable trades.</p>
  <p>The commissioner will prioritize owner autonomy but may investigate heavily lopsided trades for collusion, reserving the right to assess intent.</p>
</div>

<h3 class="subSectionHeading" bind:content={this.sixTwo}>6.2 Lending Players Prohibition</h3>
<div class="subBlock">
  <p>Players traded from a team cannot be re-acquired via trade within 6 weeks of the original trade. Violators are subject to collusion punishments.</p>
</div>

<h3 class="subSectionHeading" bind:content={this.sixThree}>6.3 Veto/Trade Process</h3>
<div class="subBlock">
  <p>A trade requires 7 veto votes to be overturned. Vetoes are only appropriate for collusion or egregious value mismatches (e.g., a star player for a backup kicker). Disliking a trade does not justify a veto.</p>
</div>

<!-- Section 7: Replacing Managers -->
<h2 class="sectionHeading" bind:content={this.seven}>Section 7: Replacing Managers</h2>

<h3 class="subSectionHeading" bind:content={this.sevenOne}>7.1 Removing Managers</h3>
<p>Managers cannot be removed against their will except for repeated failure to set a valid lineup or confirmed collusion. Active participation (league chat, trades, waivers) is encouraged but not mandatory for removal.</p>

<h3 class="subSectionHeading" bind:content={this.sevenTwo}>7.2 Replacing Managers</h3>
<p>When replacing a manager, commissioners will seek candidates with connections to existing managers, prioritizing those committed to dynasty leagues and active participation.</p>

<h3 class="subSectionHeading" bind:content={this.sevenThree}>7.3 Replacement Incentive</h3>
<p>New managers replacing a departed or removed manager receive a 50% reduction on their first-year buy-in.</p>

<!-- Section 8: League Finances -->
<h2 class="sectionHeading" bind:content={this.eight}>Section 8: League Finances</h2>

<h3 class="subSectionHeading" bind:content={this.eightOne}>8.1 League Dues</h3>
<p>League dues are set at $100. Managers must pay in full before the regular season. Late payments incur a 10% penalty ($10), added to end-of-year payouts.</p>

<h3 class="subSectionHeading" bind:content={this.eightTwo}>8.2 Payout</h3>
<p>League payout structure:</p>
<ul>
  <li>1st place: $1,000</li>
  <li>2nd place: $200</li>
</ul>
<p>Late payment penalties ($10 per late manager) add to the 1st place payout. If new managers join at a reduced rate (e.g., 50% for replacements), the difference is deducted from the 1st place prize.</p>

<h3 class="subSectionHeading" bind:content={this.eightThree}>8.3 Raising Dues</h3>
<p>Raising league dues requires a ⅔ majority vote. Managers unable to afford increased dues are encouraged to find a co-manager to split costs.</p>

</div>
