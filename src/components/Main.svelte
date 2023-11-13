<script>
    import Step from "./Step.svelte";
    import {goto} from '$app/navigation';

   let steps = [
        {
            name: "Z-Market Place ",
            icon: "fa-solid fa-cart-shopping",
            href: "https://servicesfe2-0.pages.dev/"
        
        },
        {
            name: "Portfolio",
            icon: "fa-solid fa-book",
        },
        {
            name: "To be continued",
            icon: "fa-solid fa-diagram-project",
        },
    ];

    let benefits = [
        {
            metric: "10x",
            name: "junior web-developer in training",
            description:
                "I'm a highly motivated individual enrolled in a coding bootcamp. My engineering background equips me with problem-solving skills and a logical mindset. The bootcamp is enhancing my technical proficiency and fostering adaptability. I aim to leverage my unique perspective to contribute meaningfully to the web development industry.",
        },
        {
            name: "sales, design and project engineer",
            description:
                "These roles collectively contribute to the success of engineering projects, with Sales Engineers engaging with clients, Design Engineers creating detailed plans, and Project Engineers overseeing project execution.",
        },
        {
            name: "an excellent communicator",
            description:
                "I excel as an excellent communicator, valuing transparency and constructive dialogue to build strong relationships and enhance productivity in any team or workspace.",
        },
    ];
</script>

<main class="flex flex-col flex-1 p-4">
    <section
        id="introPage"
        class="grid grid-cols-1 lg:grid-cols-2 gap-10 py-8 sm:py-14"
    >
        <div
            class="flex flex-col lg:justify-center text-center lg:text-left gap-6 md:gap-8 lg:gap-10"
        >
            <h2 class="font-semibold text-4xl sm:text-5xl md:text-6xl">
                Hi! I'm <span class="poppins text-blue-400">Heng Jian Yap</span>
                <br />Full Stack
                <span class="poppins text-violet-400">Developer</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My favorite tech includes <span class="text-violet-400"> JavaScript
                    (Svelte), HTML, CSS, TailwindCSS, Node.js + Express.js & PostgreSQL.</span>
            </p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </button>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/yap.png"}
                alt="Zetane Engine"
                class="object-cover z-[2] max-h-[70vh]"
            />
        </div>
        <!-- <div  class="flex p-0.5 relative max-w-[700px] w-full mx-auto">
            <div
                class="absolute inset-0 overflow-hidden rounded-md flex items-center justify-center"
            >
                <div
                    class="bg-gradient-to-r absolute inset-[-20px]  from-violet-800 to-indigo-800 specialSpin"
                />
            </div>

            <img
                src={"images/zetane-engine.jpeg"}
                alt="Zetane Engine"
                class="w-full h-full object-cover z-[2]"
            />
        </div> -->
    </section>
    <section class="py-20 lg:py-32 flex flex-col gap-24" id="projects">
        <div class="flex flex-col gap-2 text-center">
            <h6 class="text-large sm:text-xl md:text-2xl">
                A few of my creative endeavors.
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                Curious to <span class="poppins text-violet-400">see</span> my work?
            </h3>
        </div>
        <a
            href="https://www.youtube.com/@nextacademy-bestfullstackc4006"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-3 gap-12 lg:gap-10">
            <Step step={steps[0]}>
                <p>
                    Z-Market Place is a full stack service connecting marketplace  created with <strong
                        class="text-violet-400"
                        >Svelte, JavaScript, Node.js, Express.js and Prisma!</strong
                    > 
                </p>
            </Step>
            <Step step={steps[1]}>
                <p>
                    Portfolio is a website created using <strong
                        class="text-violet-400"></strong
                    >
                    <strong class="text-violet-400">Svelte, JavaScript, TailwindCSS, HTML.</strong
                    >
                     <strong class="text-violet-400"></strong>It serves as an introduction to
                     <strong class="text-blue-400">Heng Jian Yap</strong>
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                    Ongoing in creating an e-commerce website by using <strong class="text-violet-400"
                        >Svelte,JavaScript TailwindCSS </strong
                    > as front-end technology
                    <strong class="text-violet-400">Node.js, Express.js, Prisma!</strong> as backend technology.
                    
                   
                </p>
            </Step>
        </div>
    </section>
    <section
        id="about"
        class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative"
    >
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div
            class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4"
        >
            <h6 class="text-large sm:text-xl md:text-2xl">
                Want to know more?
            </h6>
            <h3 class="font-semibold text-3xl sm:text-4xl md:text-5xl">
                A bit <span class="poppins text-violet-400">about</span> me.
            </h3>
        </div>
        <p class="mx-auto poppins font-semibold text-lg sm:text-xl md:text-2xl">
            I am . . .
        </p>
        <div class="flex flex-col gap-20 w-full mx-auto max-w-[800px]">
            {#each benefits as benefit, index}
                <!-- <div class="flex flex-col gap-2 mx-auto">
                    <div class="flex items-end gap-4">
                        <p
                            class="poppins text-6xl sm:text-7xl md:text-8xl text-slate-500 font-medium"
                        >
                            {benefit.metric}
                        </p>
                        <p
                            class="text-xl sm:text-2xl md:text-3xl capitalize pb-2"
                        >
                            {benefit.name}
                        </p>
                    </div>
                    <p class="text-center italic">- {benefit.description}</p>
                </div> -->
                <div class="flex gap-6 sm:gap-8">
                    <p
                        class="poppins text-4xl sm:text-5xl md:text-6xl text-slate-500 font-semibold"
                    >
                        0{index + 1}
                    </p>
                    <div class="flex flex-col gap-6 sm:gap-8">
                        <h3 class="text-2xl sm:text-3xl md:text-5xl">
                            {benefit.name}
                        </h3>
                        <p>{benefit.description}</p>
                    </div>
                </div>
            {/each}
        </div>
        <h5 class={" text-2xl sm:text-3xl font-semibold text-center poppins "}>
            The <span class="text-violet-400">Complete</span> Package
        </h5>
        <div
            class="flex flex-col overflow-x-scroll gap-10 max-w-[800px] mx-auto w-full"
        >
            <table class="bg-white text-slate-700 rounded text-center">
                <thead class={"border-b border-solid border-slate-200  "}>
                    <tr class="">
                        <th />
                        <th class="whitespace-nowrap p-2 px-4">Candidate #1</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #2</th>
                        <th class="whitespace-nowrap p-2 px-4">Candidate #3</th>
                        <th
                            class="bg-violet-700 text-white whitespace-nowrap p-4 px-8"
                            >Me</th
                        >
                    </tr>
                </thead>
                <tbody>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Dedication</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-b border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Critical Thought</td
                        >
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr>
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Interpersonal Skills</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                    <tr class="border-t border-solid border-slate-200">
                        <td
                            class="border-r border-solid border-white pl-4 pr-8 py-4 font-semibold text-sm"
                            >Progamming Ability</td
                        >
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-xmark text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-slate-500" /></td>
                        <td><i class="fa-solid fa-check text-green-500" /></td>
                    </tr>
                </tbody>
            </table>
        </div>
        <div class="mx-auto -mt-12 italic sm:hidden opacity-50">
            <p>Scroll to see more &rarr;</p>
        </div>
        <p class="mx-auto">So why not invest?</p>
    </section>
    <footer id= "contact"
    class="py-20 sm:py-32 bg-black border-t border-solid border-violet-950 flex flex-col gap-4 sm:gap-8 justify-center items-center"
>
    <p class="px-4 py-2 bg-white text-slate-950 font-medium">
        Connect with me &darr;
    </p>
    <div class="flex flex-col gap-4 items-center justify-center">
        <!-- <div
            class="flex items-center gap-4 sm:gap-6 text-2xl sm:text-3xl md:text-4xl mx-auto"
        >
            <a>
                <i class="fa-brands fa-linkedin-in" />
            </a>
            <a>
                <i class="fa-brands fa-github" />
            </a>
        </div>
        <p class="mx-auto text-sm opacity-70">or</p>
        <p class="">Hugh_jass@gmail.com</p> -->
        <p><b class="pr-2">Email</b> heng.j.yap@gmail.com</p>
        <p><b class="pr-2">Phone</b> +60102529031</p>
        <p>
            <b class="pr-2">GitHub</b>
            <a href="https://github.com/dashboard" target="_blank" class="text-violet-400"
                >hemoiswhat<sup class=""
                    ><span class="text-xs scale-75 pl-0.5"
                        ><i
                            class="fa-solid fa-arrow-up-right-from-square text-xs scale-[75%]"
                        /></span
                    ></sup
                ></a
            >
        </p>
        <p>
            <b class="pr-2">LinkedIn</b>
            <a href="https://www.linkedin.com/in/heng-jian-yap-68716064/ " target="_blank" class="text-violet-400"
                >heng-jian-yap<sup class=""
                    ><span class="text-xs scale-75 pl-0.5"
                        ><i
                            class="fa-solid fa-arrow-up-right-from-square text-xs scale-[75%]"
                        /></span
                    ></sup
                ></a
            >
        </p>
    </div>
</footer>
</main>
