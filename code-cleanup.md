I have been working on the code in                                                   │
│   @site/src/components/pages/meets/report/responsive/                                  │
│      but there has been a lot of LLM generated text in there. I want to clean it up.   │
│                                                                                        │
│   Clean up the suggest folder with the following intent:                               │
│   - You are a principal-level software engineer experienced in making readible and     │
│   maintainable code                                                                    │
│   - Your top priority is making highly readible, and maintainable code. The            │
│   components themselves should be very easy to understand logic and a basic HTML       │
│   strucutre. In the CSS, please merge all duplicate classes and try to reduce any      │
│   duplicated / overriden code.                                                         │
│   - All props should be properly typed--don't do any typescript hacks to please the    │
│   compiler.                                                                            │
│   - Also add top level component comments describing what the component does           │
│   - component props should ONLY be the information that's need render the component    │
│   and it's children. Let's try to avoid throwing around a massive object all over the  │
│   place.                                                                               │
│                                                                                        │
│   Finally, assume that the input that meetReport is getting is [Pasted text #1 +282    │
│   lines] if that helps determine types and what data is actually needed 
