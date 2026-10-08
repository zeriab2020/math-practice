# Math Practice

A simple practice app for 6th grade math (Saxon Course 1 topics). It runs in any web browser, and there's nothing to install.

## How it works

- Pick a topic, or choose **Practice everything**.
- Each problem allows **3 tries**.
- A correct answer turns the problem green. The student can open the steps to review them.
- After **3 wrong tries**, the problem **locks** and shows the step-by-step solution.
- Locked problems mark their topic as **Needs review** on the **My report** page, so a parent can see which topics need more practice.
- Answers in the wrong format (for example, a decimal when a fraction is asked for) don't use up a try. The app shows a message explaining what format to use.

## Topics

Fractions, Decimals, Percents & Money, Ratios, Geometry, Exponents & Roots, Equations, Patterns, Measurement, Time & Estimation.

## For parents

- Progress is saved in the browser on the device being used. Use the same device and browser each time.
- On **My report → For parents**, create a 4–8 digit PIN. Use the PIN to reset a topic (or everything) so locked problems can be tried again.

## Adding questions

All questions are in the `QUESTIONS` list near the top of the script in `index.html`. Each question has:

| Field | Meaning |
|---|---|
| `id` | A unique short name, like `f17` |
| `topic` | The topic name shown on the cards |
| `type` | `num` (any equal number), `frac` (fraction in lowest terms), `exact` (exactly this fraction), `ratio`, `choice` (needs `options`), `time` (answer as `"15:05"`), `list` (needs `count`) |
| `text` | The question. Write fractions as `[[3/8]]` to show them stacked. |
| `answer` | The correct answer |
| `steps` | The explanation steps, shown after the 3rd wrong try |
| `final` | The final answer as shown in the explanation |
