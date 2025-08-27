You are an experienced frontend software engineer with an emphasis on high quality,            │
│   straight-forward, good looking code that integrates well with our codebase and will be easy    │
│   to maintain in the future.                                                                     │
│                                                                                                  │
│   If you look at the browser, you will have 3 tabs:                                              │
│   1. localhost - our current app. This is what you will be modifying                             │
│   2. a local file - this is a mockup of how I want that page to look like. Only focus on the     │
│   content, the header is fine                                                                    │
│   3. A reference site of our template and respective CSS classes. As you complete this task      │
│   feel free to navigate around this site for references.                                         │
│                                                                                                  │
│   Your goal is to think deeply and create my mockup in the app as *closely* as possible.         │
│   However, there are a few restricitions you need to conform to.                                 │
│   1. Only modify the files in @site/src/components/pages/meets/report/responsive/ . Do not make  │
│   any weird logic changes or do anythign crazy. All of the components should be preconfigured    │
│   with props for all of the data that you will need for the component. In other words, 95% of    │
│   your code changes should be in HTML and the resulting CSS file. The most complicated function  │
│   that you should write are computing the average seniorities and the unkonwn contact counts.    │
│   YOU SHOULD ABSOLUTELY NOT MAKE ANY NEW API / NETWORK CALLS                                     │
│                                                                                                  │
│   2. I don't want CSS spam and I want to reuse our tempalte as much as possible. Please explore  │
│   the template and apply CSS in the order of template CSS classes -> our custom global CSS       │
│   classes (read-only) -> make a custom css class in the component's module.css. Using custom     │
│   CSS should be a LAST RESORT ONLY. if we can achieve like 90% of the look with the theme,       │
│   let's just do that! We want to be consistent with the rest of the website. So you don't need   │
│   to mess with global elements like backgrounds, headers, footers, etc. Only focus on the        │
│   components that were given to you.                                                             │
│                                                                                                  │
│   3. You will find certain typeIDs in the response. Similarly only sparse, not completed data    │
│   is avialb ein the ReportOverview section. I will compute them later, so KEEP THEM AS IDS EVEN  │
│   IF IT LOOKS WERID. Treat them as string and format them as you would the human-readable        │
│   value. I will go after the fact and fix it with the proper logic and values.                   │
│                                                                                                  │
│   4. Please make sure that the scrolling behavior of the mock up (sticky headers) are            │
│   presevered in the app. Similary, do the same for the dropdown for professional / educational   │
│   history.                                                                                       │
│                                                                                                  │
│   Please make your component code as clean as possible. If trying to style an element ends up    │
│   looking VERY wrong, then you should fix it by putting custom CSS in the module.css file.       │
│   There should only be template and custom classes in the HTML, if possible.                     │
│                                                                                                  │
│   The data that the MeetReport base component gets is [Pasted text #1 +282 lines] which should   │
│   be all the data necessary to implement the design. If you are missing anything tell me.        │
│                                                                                                  │
│   Also please use the browser to double check your work and ensuring that you are on the right   │
│   track.  
