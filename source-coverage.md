# Source coverage

All slide numbers are 1-based. Reviewed extracted text from 82 React Basics slides, 124 JavaScript Refresher slides, and 40 React Styling slides, including tables, code, and notes. Embedded images were inspected separately. Rendered slides were checked for JavaScript Refresher slide 80 and React Basics slides 43–45; this was not a visual review of all 246 slides.

Nonofficial code questions are newly authored practice problems; their slide references identify supporting concepts rather than verbatim worked examples. The ten official questions remain unchanged.

| Language | Topic | PPTX | Slides |
|---|---|---|---|
| JavaScript | Variables | 10. JavaScript Refresher. JavaScript Refresher.pptx | 12–17, 44–45 |
| JavaScript | Objects | 10. JavaScript Refresher. JavaScript Refresher.pptx | 22–23 |
| JavaScript | Control flow | 10. JavaScript Refresher. JavaScript Refresher.pptx | 26–27 |
| JavaScript | Arrow functions | 10. JavaScript Refresher. JavaScript Refresher.pptx | 18–19, 48–49 |
| JavaScript | Arrays and map | 10. JavaScript Refresher. JavaScript Refresher.pptx | 24–25, 34–35 |
| JavaScript | DOM and callbacks | 10. JavaScript Refresher. JavaScript Refresher.pptx | 30–32, 98–99 |
| JavaScript | Destructuring | 10. JavaScript Refresher. JavaScript Refresher.pptx | 34–35, 52–53 |
| JavaScript | Spread and rest | 10. JavaScript Refresher. JavaScript Refresher.pptx | 40–41, 56–57 |
| JavaScript | Comparisons and logical operators | 10. JavaScript Refresher. JavaScript Refresher.pptx | 16–17, 38–39, 70–73 |
| JavaScript | Ternary and safe access | 10. JavaScript Refresher. JavaScript Refresher.pptx | 76–79 |
| JavaScript | Strings and numbers | 10. JavaScript Refresher. JavaScript Refresher.pptx | 82–85 |
| JavaScript | Array selection and sorting | 10. JavaScript Refresher. JavaScript Refresher.pptx | 88–90 |
| JavaScript | Classes and modules | 10. JavaScript Refresher. JavaScript Refresher.pptx | 60–67 |
| JavaScript | Errors and JSON | 10. JavaScript Refresher. JavaScript Refresher.pptx | 92–95 |
| JavaScript | Promises and async functions | 10. JavaScript Refresher. JavaScript Refresher.pptx | 100–105 |
| JavaScript | Scope and closures | 10. JavaScript Refresher. JavaScript Refresher.pptx | 108–111 |
| CSS | Selectors and declarations | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 7–8, 12, 36; React Basics slide 61 (official question) |
| CSS | Custom properties | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 5–6, 17, 34 |
| CSS | Reset and box model | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 7–8, 21–22 |
| CSS | Flexbox | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 16, 23–25 |
| CSS | Grid centering | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 7–8, 26 |
| CSS | Sizing and viewport units | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 16, 27 |
| CSS | Borders and overflow | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 28–29, 31 |
| CSS | Typography | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 5, 30 |
| CSS | Pseudo-classes and pseudo-elements | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 18, 32, 36 |
| CSS | Media queries | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 19, 33 |
| React | Imports and exports | 09. React - Basics.pptx | 5–8, 28–34, 38–39 |
| React | Components and fragments | 09. React - Basics.pptx | 5–26 |
| React | JSX expressions | 09. React - Basics.pptx | 41–54 |
| React | Styling in JSX | 09. React - Basics.pptx | 56–65 |
| React | CSS Modules | 12. React Styling Fundamentals - Global CSS and CSS Modules.pptx | 12–15, 35, 38–39 |
| React | Props | 10. JavaScript Refresher. JavaScript Refresher.pptx | 20, 28, 54, 58 |
| React | State and immutable updates | 10. JavaScript Refresher. JavaScript Refresher.pptx | 42, 46, 58, 112 |
| React | Event handlers | 10. JavaScript Refresher. JavaScript Refresher.pptx | 50 |
| React | Lists and conditional rendering | 10. JavaScript Refresher. JavaScript Refresher.pptx | 28, 36, 74, 80 |
| React | Mounting and effects | 10. JavaScript Refresher. JavaScript Refresher.pptx | 10, 106 |

## Source limits and ambiguities

- React Basics slide 43 contains a typo in its final inline template-literal example: the backtick/interpolation ordering is misplaced. The template-literal topic remains supported by the valid worked examples in slides 44–45; slides 44–45 support the template-literal/JSX concept used by the newly authored question 96. The reviewer uses the correct syntax.
- JavaScript Refresher slide 80 visibly contains `{isLive ?? <LiveBadge /> : <OfflineBadge />}`, a typo that combines `??` with a ternary colon. That expression is not used as an answer. The second example, `<p>{user?.profile?.bio ?? "No bio yet."}</p>`, is valid. Ternary questions use the examples in React Basics slides 49–51 and JavaScript Refresher slides 76–77.
- Several examples omit semicolons. Canonical reviewer statements retain them; grading accepts optional ending statement/declaration semicolons. JSX expressions and component tags do not receive invented semicolons.
- Notes contain no extra teaching content; some contain only slide-number placeholders.
- Six embedded images in React Basics are a logo and authentication screenshots (slides 1 and 77–81). No image-only exam code was found. Authentication details are excluded from the reviewer.
- No CSS ID-selector example was found. Grid questions use only the demonstrated grid centering. HTML-only, terminal setup, and Antigravity workflow questions are excluded.
- Some slide prose makes simplified general claims about truthiness, React internals, CSS Modules, and network data. The reviewer tests the concrete syntax shown, without repeating those claims as universal rules.
- All ten official practice questions are included exactly as supplied, with straight quotes. Official question 2 reduces the slide object to its requested name and age properties.

## Use and grading

Keep appdev-reviewer.html and code-questions.json together. When served over HTTP(S), the page imports its sibling JSON file automatically. For offline study, open appdev-reviewer.html directly in a browser and choose code-questions.json when prompted. No account, internet, or install is needed. Refreshing clears progress and loads the bank again; direct-open offline use prompts you to choose the JSON again.
Code checking normalizes curly quotes and accepts harmless spacing around JS/CSS/JSX syntax and optional ending statement/declaration semicolons. Case, quote style, token spelling/order, required punctuation, meaningful CSS spaces, and string/template/JSX text remain significant. Template literals are compared as exact text after curly-quote normalization, including interpolation formatting. Answers must match the canonical syntax or an explicitly listed alternate; alternate code answers are intentionally empty. Prompts specify formatting when needed; the ten official prompts remain unchanged.
Mock exams always contain 50 unique items: 17 JavaScript, 17 CSS, 16 React, including all ten official questions. Study filters do not change that composition. The optional mock exam timer pauses while you read Study Notes and resumes when you leave.
Mistake labels are character-based suggestions, not a parser diagnosis. Highlighting marks the first difference after allowed normalization. An empty answer is labeled Unanswered.
Handwritten grades are self-reported and included in results. Identification results are tracked separately so they do not inflate code-writing accuracy. Retry uses the latest missed result per question and mode; overall accuracy includes all completed attempts.
