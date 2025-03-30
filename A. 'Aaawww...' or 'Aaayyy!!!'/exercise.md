# Problem A. “Aaawww...” or “Aaayyy!!!”

You are a hardcore supporter for one of the teams at the Benelux Algorithm Programming Contest (BAPC). Unfortunately, the staff found you entering the contest area and popping other teams’ balloons. As a result, you were kicked out of the building and you will not be allowed back in until the contest is over. As a hardcore supporter, you would not want to miss the award ceremony and not know the final rank of your favorite team while everyone inside already knows! Luckily, you know a way to follow the award ceremony from outside the building.

One hour before the end of the contest, the scoreboard freezes. Since you can access the frozen scoreboard online, you know the rank of each team and for which problems they have accepted, rejected, or pending submissions. During the award ceremony, the results of all pending submissions are revealed, starting with the leftmost pending submission of the lowest ranking team with a pending submission. After every reveal, the scoreboard is updated and the next pending submission is chosen in the same way.

The BAPC is known for its great audience participation during the award ceremony. When the result of a pending submission is about to be revealed, the audience chants “Ooohhh...” in anticipation. When the submission is rejected, the audience utters a sad “Aaawww...”. When the submission is accepted, the crowd goes wild with an “Aaayyy!!!”. If an accepted submission causes a team to rise in the ranking, this chant goes on for longer. Specifically, an extra ‘y’ is added for each team they pass. For example, if they pass five teams, the audience will yell “Aaayyyyyyyy!!!” (with eight ‘y’s). While you cannot make out any words of the announcer, you can clearly hear the enthusiastic audience from outside. You want to use this to determine the final rank of your favorite team.

## Input

The input consists of:

- One line with three integers `n`, `m`, and `r` (2 ≤ `n` ≤ 100, 1 ≤ `m` ≤ 100, 1 ≤ `r` ≤ `n`), the number of teams, the number of problems, and the rank of your favorite team in the frozen scoreboard.

- `n` lines with `m` characters, each character being either `A`, `R`, `P`, or `N`, indicating that a team’s submission is either accepted, rejected, pending, or nothing. The teams are sorted by their rank in the frozen scoreboard, i.e., descending by number of accepted submissions in the frozen scoreboard, and further tie-breaking rules guarantee that all teams have a distinct rank.

- For each pending submission, one line with two strings, containing the audience chant at the reveal of the pending submission, in chronological order. The first string is “Ooohhh...” and the second string is either “Aaawww...” or “Aaayyy!!!”, with an additional ‘y’ for each team that is passed when rising in the ranking.

## Output

Output the final rank of your favorite team.

## Example

| **Input**                                                                 | **Output** |
|---------------------------------------------------------------------------|------------|
| `2 3 2`<br>`AAP`<br>`APR`<br>`Ooohhh... Aaayyyy!!!`<br>`Ooohhh... Aaawww...` | `1`        |
| `2 3 2`<br>`AAP`<br>`APR`<br>`Ooohhh... Aaayyyy!!!`<br>`Ooohhh... Aaayyyy!!!` | `2`        |
| `4 4 3`<br>`AAPP`<br>`PNAA`<br>`PPAA`<br>`NAPN`<br>`Ooohhh... Aaayyyy!!!`<br>`Ooohhh... Aaayyyyyy!!!`<br>`Ooohhh... Aaawww...`<br>`Ooohhh... Aaayyy!!!`<br>`Ooohhh... Aaayyyy!!!`<br>`Ooohhh... Aaayyyy!!!` | `1`        |
