# Down — Interactive Mockup (HW 1)

**Tagline:** Less planning. More living.

Down is a mobile-first social app concept for making plans with friends. Share an idea, see who's interested, and make a plan together.

## What is included

- **Pulse:** share an idea, mood, time, and budget with your circle so friends can see you're down.
- **Who's in:** preview a group match and reveal friends after enough people join.
- **Plan ideas:** browse sample activities and choose one for the group.
- **Flexible plans:** let friends join late, leave early, or update their plans.
- **Plan saving:** save the chosen plan and see it in the Plans screen.
- **Location-aware Explore:** with explicit browser permission, search real nearby places from OpenStreetMap within 3 km; filter by category/radius and rank using distance, vibe and local time.
- **Local date and time:** read from the user's device time zone and refresh the plan suggestions as time changes.
- **Explore, Plans and You screens:** additional navigation, recommendations, privacy settings, group switching and social-battery slider.
- **Responsive layout:** desktop presentation layout and phone-like mobile layout.

## Run the prototype

No package installation or API key is required. Internet access is needed for nearby-place search, and the page must be served from `localhost` or HTTPS for browser geolocation.

1. Download this folder or clone the repository.
2. Serve the folder on `localhost` or publish it over HTTPS, then open `index.html` in a modern browser. Opening the file directly may prevent geolocation from working.
3. On the Today screen, select **I'm down** or open the **Pulse** tab.
4. Send a Pulse. Choose **Preview who's in** to see the sample group flow.
5. Pick an idea, tap **I'm in**, and save the plan.

Most interactions run locally in the browser. Nearby search is the exception: after the user enables it and grants browser permission, the app sends the current coordinates to the public OpenStreetMap Overpass service for a one-time search. Coordinates stay in memory and aren't saved by Down; the cookie stores only the location opt-in preference. OpenStreetMap may receive the request and associated network information. Nearby results and opening hours depend on map coverage and may be incomplete. Friends, posts, messages, and group activity are sample content; the prototype has no account service or shared backend.

## Future coursework: activity and follow-through analysis

The current interface presents straightforward sample ideas. A later course exercise could compare activities using:
- overlap between anonymous time windows;
- group mood similarity;
- estimated cost and each member's budget preference;
- travel effort and flexibility of arrival/departure;
- private effort preferences;
- the group’s historical feedback on past plans.

This analysis should remain behind the social experience and should not present sample values as real predictions.

### Plan follow-through
A later supervised analysis could explore whether a plan happened, using appropriate consented examples and features such as time-window overlap, group size, cost, activity type, and flexibility. Any estimate would need evaluation and calibration before it could be shown as a real-world probability.

### Privacy and product risks to address
- Keep raw individual pulses private; reveal only aggregate alignment before the threshold.
- Explain what data is used, and let users opt out or withdraw their pulse.
- Treat availability and schedule information as private by default.
- Prevent a low predicted score from shaming a person or group; use it to improve plans, not judge friendships.
- Cold-start: begin with transparent preferences and group feedback before relying on historical behaviour.

## GitHub submission checklist

1. Create a **private** GitHub repository named `down-interactive-mockup` (or another name you prefer).
2. Upload `index.html` and `README.md` to the repository root, or push the folder with Git.
3. Open **Settings → Collaborators** (or **Collaborators and teams**) and invite the course account `tedaueb`.
4. If you prefer the terminal, from inside this folder run:

   ```bash
   git init
   git add index.html README.md .gitignore
   git commit -m "Build Down interactive mockup"
   git branch -M main
   git remote add origin https://github.com/YOUR-USERNAME/down-interactive-mockup.git
   git push -u origin main
   ```

   Replace `YOUR-USERNAME` with your GitHub username and create the empty private repository on GitHub before running these commands.
5. Open **Settings → Collaborators** (or **Collaborators and teams**) and invite `tedaueb`.
6. Copy the private repository URL and submit it to e-class.
7. Make sure the instructor has access if GitHub requires acceptance, and verify that the repo contains source code rather than just a screenshot.

## Suggested presentation story

> “Down makes it easy to share an idea, see which friends are in, and turn a group chat into an actual plan.”

## Files

- `index.html` — complete self-contained app mockup, including CSS and JavaScript.
- `README.md` — concept, interaction walkthrough, coursework notes, privacy considerations and submission steps.
