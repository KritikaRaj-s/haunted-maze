# HAUNTED MAZE — Escape the Curse

Static HTML game. Deploy the repository root to Vercel using the Other preset, with no build command.

## Google Forms setup

Create a Google Form with 12 short-answer fields for Member 1 name, Member 1 enrollment, Member 2 name, Member 2 enrollment, Team ID, Route, Result, Actual time, Penalty, Final time, Wrong answers, and Bonus.

Use the form's **Get pre-filled link** menu. Fill those fields with these placeholders in order:

`P1NAME`, `P1ENROLL`, `P2NAME`, `P2ENROLL`, `TEAMID`, `ROUTE`, `STATUS`, `ACTUAL`, `PENALTY`, `FINAL`, `WRONGS`, `BONUS`.

Use `ACTUALSEC` or `FINALSEC` instead if those times should be in seconds. `ACTUAL` and `FINAL` use mm:ss. Penalty is in seconds.

Copy the full generated docs.google.com link. In the game, open **Admin → Maze setup → Google Form prefilled link**, paste it, and press **Save & Validate**. Configure each event browser; settings and results are stored locally unless an external supported database is available. Vercel does not supply the original Claude database integration.

After each game, use **SUBMIT TO GOOGLE FORM**, review the prefilled values, and press **Submit** in Google Forms. Admin Results also offers a **FORM** link per team. Opening the form does not submit a response. Check the response count after the event. Do not submit twice for the same team.

Use a form volunteers can access, without file-upload questions. Respondents' result summaries are not needed. Keep the response sheet private to event organizers.

Form buttons remain hidden until a valid prefilled link is configured. No real result form is configured in this repository. Placeholder substitution has been tested with a sample link, not a real form submission.

The demo admin password is part of the client code and is not a secure authentication system.
