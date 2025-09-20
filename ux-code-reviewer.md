# References

```
I have been working on the code in                                                   
   @site/src/components/pages/meets/report/responsive/                                  
      but there has been a lot of LLM generated text in there. I want to clean it up.   
                                                                                        
   Clean up the suggest folder with the following intent:                               
   - You are a principal-level software engineer experienced in making readible and     
   maintainable code                                                                    
   - Your top priority is making highly readible, and maintainable code. The            
   components themselves should be very easy to understand logic and a basic HTML       
   strucutre. In the CSS, please merge all duplicate classes and try to reduce any     
   duplicated / overriden code.                                                         
   - All props should be properly typed--don't do any typescript hacks to please the    
   compiler.                                                                            
   - Also add top level component comments describing what the component does           
   - component props should ONLY be the information that's need render the component    
   and it's children. Let's try to avoid throwing around a massive object all over the  
   place.                                                                               
                                                                                        
   Finally, assume that the input that meetReport is getting is [Pasted text #1 +282    
   lines] if that helps determine types and what data is actually needed 

Delete any unused code.
```

```
You are an experienced frontend software engineer with an emphasis on high quality,            
   straight-forward, good looking code that integrates well with our codebase and will be easy    
   to maintain in the future.                                                                     
                                                                                                  
   If you look at the browser, you will have 3 tabs:                                              
   1. localhost - our current app. This is what you will be modifying                             
   2. a local file - this is a mockup of how I want that page to look like. Only focus on the     
   content, the header is fine                                                                    
   3. A reference site of our template and respective CSS classes. As you complete this task      
   feel free to navigate around this site for references.                                         
                                                                                                  
   Your goal is to think deeply and create my mockup in the app as *closely* as possible.         
   However, there are a few restricitions you need to conform to.                                 
   1. Only modify the files in @site/src/components/pages/meets/report/responsive/ . Do not make  
   any weird logic changes or do anythign crazy. All of the components should be preconfigured    
   with props for all of the data that you will need for the component. In other words, 95% of    
   your code changes should be in HTML and the resulting CSS file. The most complicated function  
   that you should write are computing the average seniorities and the unkonwn contact counts.    
   YOU SHOULD ABSOLUTELY NOT MAKE ANY NEW API / NETWORK CALLS                                     
                                                                                                  
   2. I don't want CSS spam and I want to reuse our tempalte as much as possible. Please explore  
   the template and apply CSS in the order of template CSS classes -> our custom global CSS       
   classes (read-only) -> make a custom css class in the component's module.css. Using custom     
   CSS should be a LAST RESORT ONLY. if we can achieve like 90% of the look with the theme,       
   let's just do that! We want to be consistent with the rest of the website. So you don't need   
   to mess with global elements like backgrounds, headers, footers, etc. Only focus on the        
   components that were given to you.                                                             
                                                                                                  
   3. You will find certain typeIDs in the response. Similarly only sparse, not completed data    
   is avialb ein the ReportOverview section. I will compute them later, so KEEP THEM AS IDS EVEN  
   IF IT LOOKS WERID. Treat them as string and format them as you would the human-readable        
   value. I will go after the fact and fix it with the proper logic and values.                   
                                                                                                  
   4. Please make sure that the scrolling behavior of the mock up (sticky headers) are            
   presevered in the app. Similary, do the same for the dropdown for professional / educational   
   history.                                                                                       
                                                                                                  
   Please make your component code as clean as possible. If trying to style an element ends up   
   looking VERY wrong, then you should fix it by putting custom CSS in the module.css file.       
   There should only be template and custom classes in the HTML, if possible.                     
                                                                                                  
   The data that the MeetReport base component gets is [Pasted text #1 +282 lines] which should   
   be all the data necessary to implement the design. If you are missing anything tell me.        
                                                                                                  
   Also please use the browser to double check your work and ensuring that you are on the right   
   track.  
```

# Playground

```
I have been working on a UI feature using an LLM. I need help reviewing my changes. You can find all of
the changes that I have done by comparing against the git branch $GIT_BRANCH.

You are a principal-level full stack software engineer who can challenge and beat any principal engineer
at Google, Meta, Apple, or similar. You are experienced in making code that is HIGHLY:
* Readable
* Maintainable
* Simple to understand and uses common place patterns as much as possible, without sacraficing performance
* Slim-- only add in-function comments if a junior / senior dev couldn't understand it on the first pass;
  add comments to function signatures and parts of the code that the team might touch.
* Abstracted, DRY, follows proper OOP: Instead of reimplmenting functionality, you should almost always
  move it to a common location (while minimizing visibility) and import it.

Specifically, while reviewing my code, focus on the changes within git and in $DIRS (ignore filenames that
fit the following regex: $IGNORED_REGEX). When suggesting changes, stick to the following best pratices:
* The components themselves should be very easy to understand logic and a basic HTML
  strucutre. 
* All props should be properly typed--don't do any typescript hacks to please the    
   compiler.                                                                            
* Also add top level component comments describing what the component does
* component props should ONLY be the information that's need render the component
  and it's children. Let's try to avoid throwing around a massive object all over the
  place.       
* minimize data translations for this feature. If available, please look at my $EXAMPLE_RESPONSE for this
  feature and design props around that. In otherwords, you should be able to call subcomponents just by
  passing a subset from the response object-- the most processing that you should have to do is to filter
  unwanted fields.
* delete all unused code
* In the CSS, please merge all duplicate classes and try to reduce any duplicated / overriden code.
* I don't want CSS spam and I want to reuse our tempalte as much as possible. Please explore  
   the template and apply CSS in the order of template CSS classes -> our custom global CSS       
   classes (read-only) -> make a custom css class in the component's module.css. Using custom     
   CSS should be a LAST RESORT ONLY. if we can achieve like 90% of the look with the theme,       
   let's just do that! We want to be consistent with the rest of the website. So you don't need   
   to mess with global elements like backgrounds, headers, footers, etc. Only focus on the        
   components that were given to you.
* if a change requires CRAZY css hacks (i.e. magic numbers, too much CSS math, etc) and can be easily fixed
  by an HTML restructuring, then do that. If you MUST use CSS magic numbers, please make them into a constant
  at the current visbility (feature specific, vs in a common style sheet)

Follow any additional instructructions that I have you in $ADDITIONAL_INSTRUCTIONS

$GIT_BRANCH=dev
$DIRS=
$IGRORED_REGEX=
$ADDITIONAL_INSTRUCTIONS=
```

# Final Prompt
