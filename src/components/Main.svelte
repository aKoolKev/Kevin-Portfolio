<script>
    import Step from "./Step.svelte";

    let steps = [
        {name: 'PsychRoadMap', icon: 'fa-solid fa-brain', href:"https://psychroadmap.netlify.app/"},
        {name: 'Math Success Center', icon: 'fa-solid fa-chalkboard', href:"https://mathsuccesscenter.netlify.app/"},
        {name: 'Chess Notation Trainer (In-progress)', icon: 'fa-solid fa-chess', href:"https://akoolkev.github.io/ChessBoardVisionTrainer/"}
    ];

    let benefits = [
        {name: 'a holder of a Bachelor of Science for Computer Science', description: 'I attended Lindenwood University from (AUG 2021 - MAY 2025) where I obtained my degree in Computer Science as well as a Minor in Mathematics.'},
        {name: 'an excellent communicator and team player', description: 'After leading a large team as the project manager and scrum master, I\'ve developed and hone my new profound skills to better collabrate with people in all areas of work from leading to being a reliable team mate.'},
        {name: 'hungry for opportunities to continue learning', description: 'Although I completed my education, I am always edgar to continue learning about the everchanging field of technology and apply them!'}
    ]


</script>

<!-- The first section: Name, Bio, Get in touch button, and profile image -->
<main class="flex flex-col flex-1 p-4">

    <!-- The first section: Name, Bio, Get in touch button, and profile image -->
    <section id="introPage" class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14">

        <div class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10">

            <!-- Name -->
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">Hi! I'm <span class="poppins text-violet-400">Kevin</span> Dong <br/> Full Stack <span class="poppins text-violet-400">Developer</span></h2>

            <!-- Bio -->
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400">favorite tech</span> includes Svelte/SvelteKit, TailwindCSS, Node.js, & Supabase!
            </p>

            <!-- Get in touch button -->
            <a class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950 cursor-pointer" href="https://www.linkedin.com/in/kevindong7" target="_blank">
                <div class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"></div>
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </a>
        </div>

        <!-- Profile picture -->
        <div class="relative shadow-2xl grip place-items-center">
            <img src={"images/profile.png"} alt="Profile image" class="object-cover z-[2] max-h-[70vh] mb-2"/>
        </div>
        
    </section>


    <!-- The second section: Projects -->
    <section id="projects" class="py-20 lg:py-32 flex flex-col gap-24">

        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-lg sm:text-xl md:text-2xl">
                A few of my creative endevors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppin text-violet-400">see</span> my work?
            </h3>
        </div>

        <a href="#" target="_blank" class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200">
            <i class="fa-brand fa-github"></i>
            <p>Visit my Github</p>
        </a>
        
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <!-- Project 1: PsychRoadMap -->
            <Step step={steps[0]}>
                <ul class="list-disc text-left leading-relaxed">
                    <li> 
                        Led and coordinated a cross-functional team of seven as <strong class="text-violet-400">Project Manager</strong> through the entire software development lifecycle.
                    </li>
                    <li>
                        Actively work alongside with the <strong class="text-violet-400">Lindenwood University Psychology Department</strong> to design and deliver an <strong class="text-violet-400">interactive web tool</strong> that connects knowledge and skills that LU students have developed in their courses (or will develop in future courses) to <strong class="text-violet-400">potential employment opportunities</strong>.
                    </li>
                    <li>Implemented an <strong class="text-violet-400">Agile-Scrum lifecycle</strong> to organize tasks, manage sprints, track progress, and facilitate team collaboration using tools like <strong class="text-violet-400">Jira</strong> and <strong class="text-violet-400">Github</strong>.</li>
                    <li>Facilitated daily stand-ups, sprint planning, and retrospectives to ensure steady progress and team alignment.</li>
                </ul>
            </Step>

            <!-- Project 2: Math Success Center -->
            <Step step={steps[1]}>
                <ul class="list-disc text-left leading-relaxed">
                    <li> 
                        <strong class="text-violet-400">Creator</strong> (Solo dev)
                    </li>
                    <li>
                        Developed a fully responsive website using <strong class="text-violet-400">Svelte</strong>, <strong class="text-violet-400">JS</strong>, <strong class="text-violet-400">Flowbite</strong>, & <strong class="text-violet-400">Tailwind CSS.</strong>.
                    </li>
                    <li>Collaborated with the <strong class="text-violet-400">Director of the Lindenwood University Math Success Center</strong> to design and launch a responsive website that raises awareness of free tutoring services and provides resources for students.</li>
                    <li>Featured on the official <strong class="text-violet-400">Lindenwood University website</strong> for its contribution to student academic support.</li>
                </ul>
            </Step>

            <!-- Project 3: Chess Notation Trainer -->
            <Step step={steps[2]}>
                <ul class="list-disc text-left leading-relaxed">
                    <li> 
                        <strong class="text-violet-400">Creator</strong> (Solo dev)
                    </li>
                    <li>
                        A tool to help increase chess player's board vision and aid with visualizing the board notation.
                    </li>
                    <li>Current tech stack: <strong class="text-violet-400">HTML</strong>, <strong class="text-violet-400">JS</strong>, & <strong class="text-violet-400">Tailwind CSS</strong>.</li>
                    <li>Future features:
                        <ul class="list-disc leading-relaxed">
                            <li>Using a modern framework such as <strong class="text-violet-400">SvelteKit</strong>.</li>
                            <li>Connect to a database such as <strong class="text-violet-400">Supabase</strong> to store user score, progress, and authentication.</li>
                            <li>Implement <strong class="text-violet-400">AI</strong> and <strong class="text-violet-400">Machine learning models</strong> to monitor user's performance.</li>
                        </ul>
                    </li>
                </ul>
            </Step>
        </div>
    </section>

    <!-- The third section: About me -->
    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <div class="flex flex-col gap0-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700
        after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
            <h6 class="text-lg sm:text-xl md:text-2xl">Want to know more?</h6>
            <h3 class="font-semibol text-3xl sm:text-4xl md:text-5xl">A bit <span class="poppins text-violet-400">about</span> me.</h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">I am ...</p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <div class="flex gap-6 sm:gap-8">
                    <p class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"> 0 {index+1}</p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">{benefit.name}</h3>  
                        <p>{benefit.description}</p>  
                    </div>
                </div>
            {/each}
        </div>

        <h5 class="text-2xl sm:text-3xl font-semibold text-center poppins">The <span class="text-violet-400">Complete</span> Package</h5>
        <div class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full">
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class="border-b border-solid border-slate-200">
                    <tr class="">
                        <th></th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th class="whitespace-nowrap bg-violet-700 text-white p-4 px-8">Me</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">Dedication</td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>

                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">Critical Thought</td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>

                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">Interpersonal Skills</td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>  
                    
                    <tr class="border-b border-solid border-slate-200">
                        <td class="border-r border-solid pl-4 pr-8 py-4 font-semibold text-sm whitespace-nowrap">Problem Solving</td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-xmark text-slate-500"></i></td>
                        <td><i class="fa-solid fa-check text-green-500"></i></td>
                    </tr>  
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
</main>