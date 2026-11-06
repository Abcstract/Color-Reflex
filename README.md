# Color Reflex

Color Reflex is a browser-based reaction-time experiment. Participants wait for a large button to appear in the center of a colored screen, then click it as quickly as possible.

The project is self-contained: there are no external libraries, databases, or installations required.

## What is being studied?

This project studies whether the color of the screen affects human visual reaction time.

The experiment uses five screen-color conditions:

- Red
- Blue
- Green
- Black
- White

Reaction time is the dependent variable and is measured in milliseconds from the moment the button appears to the moment the participant clicks it.

Each color appears three times, creating 15 valid trials per test. The same color does not appear twice in a row, and every color appears once before the next round begins. If a participant clicks before the button appears, that attempt is marked void, the participant waits three seconds, and the color is rescheduled later so the test still contains 15 valid trials.

## Statistical analysis: one-way ANOVA

The independent variable is **screen color**, with five levels: red, blue, green, black, and white. The dependent variable is **reaction time in milliseconds**.

A one-way ANOVA can be used to test whether the mean reaction time differs across the five color conditions.

### Hypotheses

- **Null hypothesis:** The mean reaction time is the same for all five colors.
- **Alternative hypothesis:** At least one color has a different mean reaction time.

The results page reports the overall mean, fastest and slowest reactions, the reaction time for every trial, and the mean reaction time for each color. Those values can be exported with the **Copy results** button and entered into a statistical program for ANOVA.

If the same participant completes every color condition, the statistically appropriate version is usually a **one-way repeated-measures ANOVA**, because the observations come from the same participant. If each reaction comes from a different participant, an ordinary one-way ANOVA may be appropriate.

## Run locally

1. Download or clone this repository.
2. Open `index.html` in a modern web browser.
3. Click **Begin test**.

No server or installation is required for basic use.
