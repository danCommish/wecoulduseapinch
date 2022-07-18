<script context="module">
	export const prerender = true;
</script>

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
    <h1 class="noUnderscore">WE COULD USE A PINCH LEAGUE CONSTITUTION</h1>
    
    <h2 class="noUnderscore">TABLE OF CONTENTS</h2>
    
    <h3 class="noUnderscore clickable" on:click={() => goToSection(one)}>Article I: Governing Body</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(two)}>Article II: League Members</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(three)}>Artcile III: League Setup</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>A:League Fees</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>B:Payout</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>C:Rosters</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>D:Scoring</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(four)}>Article IV: Draft</h3>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>A:Draft Process</h4>
        <h4 class="noUnderscore clickable" on:click={() => goToSection(threeOne)}>B:Keepers</h4>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(five)}>Article V: Regular Season</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(six)}>Article VI: Playoffs</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(seven)}>Article VII: Trades</h3>
    <h3 class="noUnderscore clickable" on:click={() => goToSection(seven)}>Article VIII: Waivers</h3>
    <hr />
    
    <h2 class="sectionHeading" bind:this={one}>Article I: Governing Body</h2>
      <ol type="A">
        <li>At the beginning of each season, the previous League Commissioner (henceforth referred to: LC) will continue his/her role unless he/she has relinquished said role.</li>
        <li>During the season, the LC will be responsible to efficiently run the day-to-day operations of the We Could Use a Pinch (Henceforth referred to: WCUP) and will be required to interpret the appropriate course of action based on the terms outlined in this Constitution and by Sleeper.com.</li>
        <li>The commissioner does not have autonomous rule over the league and may be removed from office through a unanimous vote by the league.</li>
        <li>LC will appoint a co-commissioner, who can retain or relinquish duties each season</li>
        <li>New members will be admitted to WCUP in pairs as to insure an even number of members.</li>
      </ol>

    <h2 class="sectionHeading" bind:this={two}>Article II: Leauge Members</h2>
      <ol type="A">
          <li>There will be 12 teams for each season, no more, no less.</li>
          <li>All interested members from the previous season have the right to retain their franchise as long as they have not been banned by the league committee.</li>
          <li>Bannings will be instituted by the LC based on a majority vote and must be upheld for a minimum of 2 seasons.</li>
          <li>Bannings will be issued as a result of franchise negligence, failure to pay league fees in a timely manner and/or for reasons currently beyond comprehension but for which, at said time, the LC deems banning appropriate through majority vote.</li>
          <li>If a member chooses to leave the league, they are not automatically guaranteed to gain their spot when and if they want to re-join.</li>
          <li>League Communication will occur in the Sleeper league chat.</li>
        </ol>

    <h2 class="sectionHeading" bind:this={three}>Article III: League Setup</h2>
    <ol type="A">
    <li>
        <p>League Fees</p>
        <ol>
            <li>
                <p>Will equal the decided upon entry fee for the league plus fees associated with league setup.</p>
            </li>
            <li>
                <p>Will be due by the day of the draft.</p>
            </li>
            <li>
                <p>Failure to pay league fees by the time of the draft will result in league banning.</p>
            </li>
        </ol>
    </li>
    <li>
        <p>Payout Structure (based on a $20 buy-in)</p>
        <ol>
            <li>
                <p>1st Place - $150 (60%)</p>
            </li>
            <li>
                <p>2nd Place - $75 (30%)</p>
            </li>
            <li>
                <p>3rd Place - $25 (10%)</p>
            </li>
            <li>
                <p>Most Points - You will receive the penalty money from the season</p>
            </li>
        </ol>
    </li>
    <li>
        <p>Rosters</p>
        <ol>
            <li>
                <p>Each team will consist of 1 QB, 2 RB, 2 WR, 1 TE, 1 RB/WR/TE, 1 K, 1 IDP, &amp; 5 bench roster spots.</p>
            </li>
            <li>
                <p>Each team will have 2 Injured Reserve Spot.</p>
            </li>
        </ol>
    </li>
    <li>
        <p>Scoring</p>
        <ol>
            <li>
                <p>Head to head format. &nbsp;Schedule will be generated by Sleeper at Random..</p>
            </li>
            <li>
                <p>Passing:</p>
                <ol>
                    <li>
                        <p>Every 1 passing yard = .04 points (1 point for every 25 yards)</p>
                    </li>
                    <li>
                        <p>TD Pass = 4 Points</p>
                    </li>
                    <li>
                        <p>2pt Passing Conversion = 2 points</p>
                    </li>
                    <li>
                        <p>Interceptions = -2 points</p>
                    </li>
                    <li>
                        <p>1 extra point when passing yards &gt;= 300</p>
                    </li>
                    <li>
                        <p>2 extra points when passing yards &gt;=500</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Rushing:</p>
                <ol>
                    <li>
                        <p>Every one rushing yard = .1 points (1 point for every 10 yards)</p>
                    </li>
                    <li>
                        <p>Rushing TD = 6 points</p>
                    </li>
                    <li>
                        <p>2pt Conversion = 2 points</p>
                    </li>
                    <li>
                        <p>1 extra point when rushing yards &gt;=100</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Receiving:</p>
                <ol>
                    <li>
                        <p>Per Reception = .5 points</p>
                    </li>
                    <li>
                        <p>Every one receiving yard = .1 points (1 point for every 10 yards)</p>
                    </li>
                    <li>
                        <p>Receiving TD = 6 points</p>
                    </li>
                    <li>
                        <p>2pt Conversion = 2 points</p>
                    </li>
                    <li>
                        <p>2 extra points when receiving yards &gt;= 150</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Miscellaneous:</p>
                <ol>
                    <li>
                        <p>Kickoff Return TD = 6</p>
                    </li>
                    <li>
                        <p>Fumble Return TD = 6</p>
                    </li>
                    <li>
                        <p>Punt Return TD = 6</p>
                    </li>
                    <li>
                        <p>Fumble Lost = -2</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Kicking:</p>
                <ol>
                    <li>
                        <p>PAT Made = 1 point</p>
                    </li>
                    <li>
                        <p>PAT Missed = -1</p>
                    </li>
                    <li>
                        <p>FG Made (0-49yds) = 3</p>
                    </li>
                    <li>
                        <p>FG Made (50+) = 5</p>
                    </li>
                    <li>
                        <p>FG Missed (0-49) = -1&nbsp;</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>IDP Scoring</p>
                <ol>
                    <li>
                        <p>IDP Safety = 3 Points</p>
                    </li>
                    <li>
                        <p>IDP Forced Fumble = 3 Points</p>
                    </li>
                    <li>
                        <p>IDP def_td = 6 points</p>
                    </li>
                    <li>
                        <p>IDP_blk_kick = 3 points</p>
                    </li>
                    <li>
                        <p>IDP_int = 6 points</p>
                    </li>
                    <li>
                        <p>IDP_qb_hit = 1 Points</p>
                    </li>
                    <li>
                        <p>IDP_pass_def = 3 Points</p>
                    </li>
                    <li>
                        <p>IDP_tkl_loss = 2 Points</p>
                    </li>
                    <li>
                        <p>IDP_fum_rec = 3 Points</p>
                    </li>
                    <li>
                        <p>IDP_sack = 6 Points</p>
                    </li>
                    <li>
                        <p>IDP_tkl_ast = 1 Points</p>
                    </li>
                    <li>
                        <p>IDP_tkl_solo = 2 Points</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Bonus Points</p>
                <ol>
                    <li>
                        <p>100-199 Yard Rushing Game = 2 points</p>
                    </li>
                    <li>
                        <p>200+ Yard Rushing Game = 3 points</p>
                    </li>
                    <li>
                        <p>100-199 Yard Receiving Game = 2 points</p>
                    </li>
                    <li>
                        <p>200+ Yard Receiving Game = 3 points</p>
                    </li>
                    <li>
                        <p>400+ Yard Passing Game = 4 points</p>
                    </li>
                    <li>
                        <p>1st Down Gained = .5 points</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Fractional Points are allowed</p>
            </li>
            <li>
                <p>Negative Points are allowed</p>
            </li>
        </ol>
    </li>
    <li>
        <p>Platform - The league will operate on the Sleeper Fantasy Football Platform.</p>
    </li>
</ol>

    
    <h2 class="sectionHeading" bind:this={four}>Article IV: Draft</h2>
    <ol type="A">
    <li><br>
        <ul>
            <li>
                <p>Draft Process</p>
            </li>
            <li>
                <p>The draft order will be determined by the final standings of the previous season. The top 6 will head to the playoffs, the bottom 4 will start a losers playoff.</p>
            </li>
            <li>
                <p>A weighted lottery will take place to determine the order of selection of draft spots. The winner of the loser&rsquo;s bracket receives the highest chances of winning the lottery.</p>
            </li>
            <li>
                <p>The draft selection will happen at minimum 7 days prior to the draft.</p>
            </li>
            <li>
                <p>Once the draft order is determined, the draft order will be in &ldquo;snake&rdquo; format (1st pick in round 1, has last pick in round 2, and so forth).</p>
            </li>
            <li>
                <p>The draft date will&nbsp;always&nbsp;be the Labor Day Weekend; the location will be determined yearly.</p>
            </li>
            <li>
                <p>The draft will be a live draft.</p>
            </li>
            <li>
                <p>The draft will be 15 rounds.</p>
            </li>
            <li>
                <p>The draft will have one 30 minute break after round 7</p>
            </li>
            <li>
                <p>If a manager attempts to draft a player who has already been selected, they will pay $5 into the pot.</p>
                <ol>
                    <li>
                        <p>They must also be mocked without mercy for the remainder of the draft.</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Managers must&nbsp;draft&nbsp;an entire team, filling out all roster spots from QB-K (Conner Rule)</p>
            </li>
            <li>
                <p>If one cannot attend the draft, either in person or via webcam, they will be auto drafted.&nbsp;</p>
                <ol>
                    <li>
                        <p>We will use Fantasy Football Calculator player rankings and draft best available for starting lineup.&nbsp;</p>
                        <ol>
                            <li>
                                <p>We will draft your starting lineup (including kicker and defense) before filling up your bench.&nbsp;</p>
                            </li>
                        </ol>
                    </li>
                    <li>
                        <p>If you want to submit your own player rankings, we can do that as well.</p>
                    </li>
                </ol>
            </li>
        </ul>
        <ol>
            <li>
                <p>Keepers</p>
            </li>
        </ol>
        <ul>
            <li>
                <p>Players drafted in rounds 1 and 2 of the draft are&nbsp;ineligible&nbsp;to be kept. This rule is in place to increase parity and competition in the league.</p>
                <ol>
                    <li>
                        <p>Keepers under contract are exempt from this rule</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>A player must be on the teams roster at the conclusion of the season to be kept by an owner.</p>
            </li>
            <li>
                <p>Keepers are only allowed to be kept by a team for a maximum of&nbsp;three consecutive seasons. The contract clock began prior to the&nbsp;2018 season. (ex. Dan had Stefon Diggs and kept him into 2018, thus 1 year is gone off the players &lsquo;contract&rsquo;. If Dan keeps Diggs again in 2019, he will have 2 years off his &lsquo;contract&rsquo; allowing Dan to only keep Diggs for one more year (if he chooses so)).</p>
            </li>
            <li>
                <p>Keepers must be declared by Sunday August 21, 2022 at 7PM</p>
            </li>
            <li>
                <p>Each franchise can keep a maximum of one players from the previous year&rsquo;s roster, but is not required to keep any players.</p>
            </li>
            <li>
                <p>To be eligible as a keeper, player must either be drafted in the initial draft OR picked up prior to&nbsp;Week 6&nbsp;of the season. Player must also be on the owner&rsquo;s roster at the end of regular season play. In the case of IR, IR player must have been drafted in the initial draft to be eligible.</p>
                <ol>
                    <li>
                        <p>Example 2018 Darius Guice (RB, WSH) tore an ACL in preseason and was out the entire 2018 season. To be eligible to be kept by a manager, you must have&nbsp;DRAFTED&nbsp;Guice (as long as it wasn&rsquo;t in rds 1 or 2).&nbsp;</p>
                    </li>
                    <li>
                        <p>Traded players that were originally drafted after round 2 by one team may be kept by the acquiring team.</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Players kept from the original draft will be re-drafted at draft spot -1 from previous year. You MUST DRAFT a player for this rule to apply, otherwise the below applies.</p>
                <ol>
                    <li>
                        <p>2018 Jay Ajayi was drafted 4.10 - if kept he will be a Rd 3 pick.</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Players picked up between draft and Week 6 will be re-drafted at ADP +1.</p>
                <ol>
                    <li>
                        <p>George Kittle was picked up wk 2 in 2018 by Chris, he will be drafted at his ADP (3.5)+1 Round 4.</p>
                    </li>
                </ol>
            </li>
            <li>
                <p>Players drafted in Rounds 1 and 2 of previous year&rsquo;s draft are ineligible for ALL teams.</p>
            </li>
        </ul>
        <ol></ol>
    </li>
</ol>

    <h2 class="sectionHeading" bind:this={five}>Section 5 Tanking Policy</h2>
    
    <h3 bind:this={fiveOne}>5.1 League Tanking Policy</h3>
    <p>No team may intentionally leave starting roster spots empty. Any evidence of intentionally leaving roster spots empty in order to improve your draft position may be subject to punishment, including but not limited to the forfeiture of draft selections.</p>

    <h2 class="sectionHeading" bind:this={six}>Section 6 Replacing Managers</h2>
    
    <h3 bind:this={sixOne}>6.1 Removing Managers</h3>
    <p>Short of continuously failing to set a valid lineup, or confirmed collusion, no manager can be removed against their will. Participation, through the league chat, trade offers, and the waiver wire, is strongly encouraged but generally grounds for removal.</p>
    
    <h3 bind:this={sixTwo}>6.2 Replacing Managers</h3>
    <p>When a manager needs to be replaced, the commisiooners will try to find a suitable candidate with some connection to at least a portion of the existing managers. Priority will be placed on managers who are eager to take on a dynasty commitment and will be very active within the league.</p>
    
    <h3 bind:this={sixThree}>6.3 Replacement Incentive</h3>
    <p>In the event that a manager chooses to quit the league or is removed by a comissioner, an incoming manager is offered a 50% reductioon on their first year buy-in.</p>

    <h2 class="sectionHeading" bind:this={seven}>Section 7 League Finances</h2>
    
    <h3 bind:this={sevenOne}>7.1 League Dues</h3>
    <p>League dues are set at {dues}$. Dues are collected through <a href="https://www.leaguesafe.com/league/3949641">LeagueSafe</a> and collection will be sent out no later than the first of August. All managers must be fully paid up before the start of regular season. In the event that a manager fails to pay before the deadline, a 10% penalty will be addd to their payment and will go towards the payouts at the end of the year.</p>
    
    <h3 bind:this={sevenTwo}>7.2 Payout</h3>
    <p>League payout is structured as follows:</p>
    <ul>
        <li>1st place: {dues * 8}$</li>
        <li>2nd place: {dues * 3}$</li>
        <li>3rd place: {dues}$</li>
    </ul>
    <p>In the event that a manager was fined due to late payment, their extra fee will be added to the winner's payout. Similarly, if new managers come into the league and the payout is smaller, the difference will come out of the winner's prize.</p>
    
    <h3 bind:this={sevenThree}>7.3 Raising Dues</h3>
    <p>A ⅔ majority vote is required in order to raise league dues. In the event that a manager is no longer financially comfortable with the buyin, finding a co-manager to split the cost is reccomended.</p>

</div>
