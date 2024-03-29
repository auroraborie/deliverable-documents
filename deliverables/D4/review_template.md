## D4 - Project Review

Please fill in the template below. Some suggestions have been provided to help you understand how to answer each segment.

Before submission, please replace the suggestions (in italics) with your answers. You can keep the prompts though.

### Project Name: EduNexus
### Team Name, Team Number: EduNexus, Team 37
### Github Link: https://github.com/csc301-2024-s/deliverable-1-37-edunexus

### Project Summary:

EduNexus is an academic support application which aids educators in underprivileged areas to easily track student grade records and personalize exams report generation. The project aims to improve the administrative organization of schools through automated workflows and digital scalability. They have implemented key features such as automated report generation, student performance analysis, and secure data management to create a user-friendly and non-technical experience for ease of use by educators. 

### Introduction & Overview of the problem and the product:

I was able to infer what problem this project is trying to solve through context clues. However, more context in the README of the repo would have been helpful and more convincing about how important this application is. Specifically, by providing some facts and figures or examples of the places and the educators who may have difficulty in student record management that would find this project helpful. 

I was able to get an overview of the project through watching both the demo video and readme file. 

This project has many similar functionalities to other academic support tools, such as showing student performance analytics and adding different types of users. However, this project can differentiate itself by being designed for helping educators in technologically underserved areas, and as such incorporated more user-friendly and automated workflows. As well, anticipating the scarcity of internet access, EduNexus is developed to run packaged locally on the computer. 

More competitive analysis between their product and other educational support tools on the market would help me get more information on how their product differs and is more advantageous to the user. 

### Demo of the application:

I found the demo video to bring forward impactful points on the features of their product. 

Key points include:
- EduNexus is designed for technological scarcity through being able to run entirely on a local machine
- Designed for different level of users (admin/teacher)
- Users can go through their workflows with ease depending on their position

Additionally, the ideas were presented with a clear voice and the video production was edited with minimal paused spaces for ease of understanding.  

The team demonstrated most but not all of the documented key features on the README. One feature was the generate PDF functionality which was not implemented yet due to Electron packaging issues, which is the framework they used to develop the application. Another was the ability to add students to a class, which they say will be developed for D5. The rest of the features worked well such as viewing student grade trends and downloading the class list. 

The demo helped me get a good understanding of this application by taking me through the typical workflows through the point of view of an administrator and teacher. This contrast through the different users also clearly demonstrated the different access levels granted to educators based on their position. 

Key features noted:
- Administrators can add classes and assign teachers to the various classes, which is typical of the position
- Teachers can only see the classes which they have been assigned, which makes sense for privacy and work related concerns

The demo video was overall helpful and informative, though I had remaining questions on the design choices behind demonstrated features that would me understand how to use the tools better. 

- Why use a bar chart for the graphic display over other charts?
- Why choose to implement only admin and teacher user types and not students?
- Why can a teacher not add any students to a class themselves? 

### Technical Discussion & Key Learnings:

From the demo and looking at their codebase, EduNexus was built on Electron, which embeds Chromium (renders UI) and Node.js (runs backend). The main benefit of Electron was being cross platform operational for its deployment (on macOS, Windows, and Linux). The UI was created using React.

The frontend code is in the renderer.js app and the backend code is in the main.js files. The Electron package allows a contextBridge between frontend and backend in order to send data securely between them. 

Key learnings presented: 
1. Earlier adoption of pair programming
2. More in person coding meetings for peer support
3. Use Tauri instead of Electron as a framework

I believe that these key learnings make sense and are achievable. The first two are achievable as team members already have set up meetings and can simply pivot to meeting in person by finding a common workplace which are numerous on campus. The team can make it concrete by setting a specific date each week for the in person coding sessions. 

I think using Tauri instead of Electron can also help improve the project as Tauri is a lighter application (as it uses less memory and CPU processing power), so it runs faster than Electron. As well, Tauri is more secure than Electron as it uses a memory safe language called Rust. This may improve their application by enhancing performance speed and data security which is important when working in the domain of student records. Given the timeframe, this key learning may not be achievable but can be a future implementation to help improve the project. 

Looking through the project's codebase, in the path: test/specs/test.e2e.js, I can see that testing is implemented but no comments are left. Testing was not mentioned in the demo as well. More information on the team's testing coverage would I believe help the audience understand the functional features of their code versus the ones still in development, and inform future contributors of where in the codebase they need to fix or be mindful of when using. 


### Project Documentation:

The readme was easy to follow as it was well formatted and had concise points on the features, installation, techstack, and collaboration standards. This helped the viewer get a good background on the features of the application and how they can install and/or contribute the application themselves. 

It was easy to read and follow the readme as the document followed good formatting with prominent titles and subpoints. 

Overall, there were no technical or major writing errors. The only point that may lead to confusion was that under key features, they list PDF generator as a feature. However, this is not yet implemented. 

Since some of the features are still in development, it may be more clear if the team included a 'to be implemented' section and 'implemented' features section. This can also help in informing future collaborators of the work that they can do, and avoid using the functionalities that do not yet work. 

The use of diagrams would also help improve the quality of the documentation. Visuals of the backend architecture in the readme, along with pictures of the UI and its graphical display rendering would help the first time user understand the application more hollistically. 

### Project Deployment:

I followed their instructions and was able to clone and download the necessary packages onto my local machine. 

Most of the features ran as expected. Other than the features mentioned in the demo that were still in development (such as how PDFs cannot be generated currently, and that there is no way to add students to a class) the only error I encountered was when I created a new teacher user, assigned it a class and logged in, the entire school's data was displayed instead of the single class I assigned to the teacher. Also the label read 'John Doe' instead of the name I typed in. 

I tested the key features that were mentioned in the readme file, and additionally the authentication feature for data security. The key features worked as demonstrated in the demo video, and I was able to login to the application under different user levels.  

Some edge cases to consider are:

1. Teachers may want to be able to get alerts when a student is falling behind in their class. In the edge case when a student's grade drops suddenly, it may be helpful to notify the teacher so they can figure out how to help the student. 

2. Currently, the application only works to visualize the entire class' grades however teachers are also responsible for individual students as well. So to be able to monitor a individual student's grades over time as well to see improvement or decline so that educators can help accordingly is an edge case that can be considered.

From my experience the UI of this product is well structured and coloured from a user perspective. It follows common web app layout convetions such as having a toolbar on the left side of the screen but it is not similar in my oppinion to any products similar to this project. 

After adding a new class and teacher, it would be useful to also be able to see it in the admin view. Currently, when I added these new pieces of information and searched for it from the admin account, they do not display. In a school setting, admin staff should be able to see the new classes from the application.

### Misc.:
An additional point to consider is that students may be a user group that the application can also consider as they may have difficulty keeping track of their test scores from the past. They can also benefit from having their records in a secure place for access and use it to calculate their GPAs.



