# Maria Fiodorova

## Location
Austin, TX
___

## Contact Information
Email: [mf@gmail.com](mailto:mf@gmail.com)
Phone number: [+1 512 1234567](tel:+15121234567)
GitHub: [mariarp10](https://github.com/mariarp10)
Codewars: [CodeMochi](https://www.codewars.com/users/CodeMochi)
Discord: [maria_72134](https://discord.com/users/1389296278059356270)
___

## Summary
Howdy ho! 👋🏻
I'm Maria, a Front-End Engineer with a pythonic twist, and a seasoned high-tech professional with background as a Product Owner. Over the past 1.5 years, I have built solid expertise in JavaScript, HTML5, CSS, TypeScript, RESTful APIs, OOP, and React.js, focusing on creating reliable, user-centered solutions.
I bring to my developer role the same strengths that made me successful as a Product Owner: clear communication with stakeholders, empathy for end-users, and strong analytical thinking. 
I thrive on solving complex problems and delivering practical, low-hanging fruit solutions that balance technical feasibility and user impact.

___

## Skills
- HTML5, CSS, JavaScript ES6
- TypeScript
- React.js, testing React apps
- Git, GitHub
- Chrome DevTools, Debugging
- Figma for web development
- OOP, RESTful API
- Advanced Python
- Algorithms
___

## Code Examples
```
/**
 * Finds the unique number in an array where all other numbers appear more than once.
 *
 * @param {number[]} arr - An array of numbers that contains exactly one unique number.
 * @returns {number} The unique number that appears only once in the array.

 @timecomplexity O(n) - It loops through the array twice: once to count and once to find the unique number.
 */
function findUniq(arr) {
  const counter = new Map();
  let unique;
  for (const num of arr) {
    if (!counter.has(num)) {
      counter.set(num, 1);
    } else {
      counter.set(num, counter.get(num) + 1);
    }
  }
  for (const [key, value] of counter.entries()) {
    if (value === 1) {
      unique = key;
    }
  }
  return unique;
}
```

```
/**
 * Solves a quadratic equation of the form ax² + bx + c = 0.
 * Uses a cache to store square root values for repeated discriminants.
 *
 * @param {number} a - The coefficient of x².
 * @param {number} b - The coefficient of x.
 * @param {number} c - The constant term.
 * @returns {(number[]|undefined)} An array of real solutions, or undefined if there are no real solutions.
 */
const sqrtCache = new Map();

function solveQuadratic(a, b, c) {
  if (a === 0) {
    if (b === 0) return;
    return [-c / b];
  }

  const D = b ** 2 - 4 * a * c;

  if (D < 0) return;
  if (D === 0) return [-b / (2 * a)];

  let sqrtD;
  if (sqrtCache.has(D)) {
    sqrtD = sqrtCache.get(D);
  } else {
    sqrtD = Math.sqrt(D);
    sqrtCache.set(D, sqrtD);
  }

  return [(-b + sqrtD) / (2 * a), (-b - sqrtD) / (2 * a)];
}
```
___

## Projects
Below are selected coursework projects that demonstrate my growing front-end development skills. Each project reflects how I’ve progressed in using modern approaches like adaptive design, CSS grids, flexbox, and animations to build responsive and visually appealing web pages. I share these to show my commitment to improving my craft and delivering polished, user-friendly experiences.

### Sales Bonus 
###### JavaScript App
The program calculates bonuses for sales reps based on their performance, and outputs a table with accumulated data on the sales reps.

**Skills:** JavaScript

**Links:** [Source Code](https://github.com/mariarp10/sales-bonus)

### Closing Tag
###### Responsive Web Page
A static landing page with animated visual elements (buttons, icon) and adaptive design for all screen sizes.

**Skills:** HTML, CSS, adaptive design, animations.

**Links:** [Deployed page](https://mariarp10.github.io/zakrivayuschiy-teg-f/) | [Source Code](https://github.com/mariarp10/zakrivayuschiy-teg-f)

### Difficult to Focus
###### Responsive Web Page with Theme Toggle
A creative static page leveraging adaptive design, dynamic themes switching, and complex grid for pictures gallery.

**Skills:** HTML, CSS, adaptive design, grid, theme toggling.

**Links:** [Deployed page](https://mariarp10.github.io/slozhno-sosredotochitsya-fd/) | [Source Code](https://github.com/mariarp10/slozhno-sosredotochitsya-fd)
___

## Work Experience

### Software Engineer
Career Transition & Ongoing Learning
_Jan 2024 - present_

Actively participating in programming bootcamps and self-directed study to build professional-level programming skills, focusing on Front-End development.

**Results and Achievements:**
- solved 2.8k+ programming challenges over the past year, strengthening problem-solving skills and algorithmic thinking
- developed 6 front-end projects applying modern approaches such as adaptive design, CSS Grid, Flexbox, and animations
- completed 3 intensive programming bootcamps within the last 18 months, practicing modern in-demand programming languages such as Python and JavaScript

Future plans include mastering server-side programming with Node.js and Django.

### Product Owner
at [Armada Labs](https://www.armadalabs.com/)
_Oct 2022 - Oct 2023_
Armada Labs is an outsourcing company that specializes in bespoke software development services for financial companies. The company has a strong focus on providing solutions for online banking, digital payment platforms, and lending companies.

**About the project:** implementing an MVP of an investment platform for a US-based client.

**Results and Achievements:**
- Conducted the Discovery Phase, transforming client documentation into a streamlined backlog in 3 weeks through wireframing, market research, and key stakeholder interviews to refine user stories. 
- Developed and delivered a robust MVP in 4 months by leading design and engineering teams, resolving tech/design challenges, planning sprints, and providing consistent updates to the client.

### Product Owner
at [Andersen Lab](https://andersenlab.com/)
_Nov 2020 - Oct 2022_

Andersen Labs is an outsourcing company with a team of 2,000+ employees who deliver full-cycle development services to clients across the US and Europe.

**About the project:** ongoing development of the company's corporate website, adding new features and lead-generation mechanics to attract potential partners.

**Results and Achievements:**
- Launched the German version of the website by leading a 6-member team and devising an adaptive process for integrating translations, securing a key client from the DACH region.
- Spearheaded technical documentation for a 2-year project from scratch by designing project-specific Confluence templates, achieving a 62% bug reduction and boosting feature delivery speed by 37%. 
- Transformed the design team's workflow with a specialized Jira template and checklist, enhancing task clarity and cutting operational time by 25%.


## Education
**Front-End Engineer**
TripleTen Software Engineering Bootcamp
_April 2025 - present_

**Python Engineer**
Self-directed Learning
_May 2024 - present_

**B.A. in Foreign Languages (English)**
Minsk State Linguistic University 
_2018-2023_
