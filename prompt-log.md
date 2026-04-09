# Prompt Log — Homework 1

## Prompt 1: Initial Project Review
- **Tool Used:** GitHub Copilot
- **Prompt:** "I am tasked with an assignment and I need your help to generate a portfolio website. Can you take a look at both the README.md and starter-template.html files?"
- **Goal:** Review assignment requirements and template
- **Result:** Examined requirements and created portfolio.html

## Prompt 2: Update Documentation & Clear Files
- **Tool Used:** GitHub Copilot
- **Prompt:** "Update the readme.md to include instructions on how to run the portfolio using python3 -m http.server 8000 and the link http://localhost:8000/portfolio.html. Clear the reflection and issues md since I want to write those myself. Update the prompt log md to include the latest chat."
- **Goal:** Document how to run the site and prepare files for manual writing
- **Result:** README updated with run instructions, issues.md and reflection.md cleared to templates

## Prompt 3: Mobile Testing Guidance
- **Tool Used:** GitHub Copilot
- **Prompt:** "How can i test the mobile site?"
- **Goal:** Get clear mobile testing instructions
- **Result:** DevTools mobile emulation workflow provided

## Prompt 4: Hide Navigation on Scroll
- **Tool Used:** GitHub Copilot
- **Prompt:** "On mobile the section that shows Home, About, Projects, and Contact seems to take too much of the screen. I want you to make it so when the user scrolls down that section goes away and when the user scrolls up they see that section will come back."
- **Goal:** Improve mobile screen space by hiding nav on scroll
- **Result:** Implemented scroll-triggered nav hide/show with transform transition

## Prompt 5: Condense Prompt Log
- **Tool Used:** GitHub Copilot
- **Prompt:** "Can you update the prompt log so matches the prompts I gave you"
- **Goal:** Make prompt log match actual user prompts given
- **Result:** Condensed to real user requests from conversation

## Prompt 6: Mobile Navigation Redesign
- **Tool Used:** GitHub Copilot
- **Prompt:** "Testing out the mobile version of the site, it still feels off to me. Instead of the menu bar disappearing or reappearing when scrolling, can the menu items be all next to each other on mobile the way they are on tablet or pc? And they should be horizontal instead of vertical. Can you also make the background for that menu bar a different color, maybe grey?"
- **Goal:** Improve mobile nav UX with horizontal layout and grey background
- **Result:** Nav now stays horizontal on mobile with grey background; removed scroll-hide behavior
- **Changes Made:** Changed nav background to #e8e8e8, removed flex-direction column on mobile, removed scroll event listener

## Prompt 7: Project Pop-Up Modal
- **Tool Used:** GitHub Copilot
- **Prompt:** "When clicking view on any of the 4 projects the current functionality will jump the user to the top of the page which feels awkward. Can you make it so clicking the View Project button opens a pop-up window with details for that project, and add an exit/close button? I do not want the button to redirect to a new page, only a pop-up window."
- **Goal:** Replace anchor jump behavior with in-page project details modal
- **Result:** Each View Project button now opens a modal with project details and a close button; no redirect occurs
- **Changes Made:** Replaced project links with buttons, added modal HTML/CSS/JS, added open/close behavior and overlay click-to-close

## Prompt 8: Fix Project Button Issue
- **Tool Used:** GitHub Copilot
- **Prompt:** "There appears to be an issue in portfolio.html and when testing out the view project button nothing happens"
- **Goal:** Diagnose and fix broken View Project popup behavior
- **Result:** Fixed parsing/script issue and restored button functionality
- **Changes Made:** Removed accidental script block near top of file, re-added modal JavaScript in the correct script section, verified no errors

