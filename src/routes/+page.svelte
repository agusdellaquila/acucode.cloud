<script>
    import "./landing.css"
    import Skill from '../components/skill.svelte';
    import Calendly from "../components/calendly.svelte";
    // import Mouse from '../components/mouse.svelte';
    import LinkedIn from '../assets/Landing/linkedin.png';
    import Github from '../assets/Landing/github.png';
    import Logo from '../assets/Landing/logo.png';
    import Underline from '../assets/Landing/underline.png';
    import Paperplane from '../assets/Landing/paperplane.png';
    import Clouds from '../assets/Landing/cloud_separator.png';
    import Cobra from '../assets/Landing/cobradenim.png';
    import Binarybrains from '../assets/Landing/binarybrains.png';
    import Stocksystem from '../assets/Landing/stocksystem.png';
    import Crown from '../assets/Landing/crown.png';

    let skills = [
        {
            name: "React",
            icon: "https://img.icons8.com/color/48/000000/react-native.png"
        },
        {
            name: "Svelte",
            icon: "https://upload.wikimedia.org/wikipedia/commons/thumb/1/1b/Svelte_Logo.svg/1200px-Svelte_Logo.svg.png"
        },
        {
            name: "Tailwind",
            icon: "https://img.icons8.com/fluency/256/tailwind_css.png"
        },
        {
            name: "Express",
            icon: "https://jsurt.github.io/jacks-portfolio/images/color-express-icon%20(1).png"
        },
        {
            name: "MySQL",
            icon: "https://img.icons8.com/color/48/000000/mysql-logo.png"
        },
        {
            name: "Power BI",
            icon: "https://upload.wikimedia.org/wikipedia/commons/thumb/c/cf/New_Power_BI_Logo.svg/2048px-New_Power_BI_Logo.svg.png"
        },
        {
            name: "Figma",
            icon: "https://img.icons8.com/color/48/000000/figma--v1.png"
        },
        {
            name: "Wordpress",
            icon: "https://img.icons8.com/color/48/000000/wordpress.png"
        },
        {
            name: "JavaScript",
            icon: "https://img.icons8.com/color/48/000000/javascript--v1.png"
        },

    ]

    let softSkills = [
        {name: "Organization"},
        {name: "Time management"},
        {name: "Teamwork"},
        {name: "Problem solving"},
        {name: "Attention to detail"},
        {name: "Punctuality"},
        {name: "Adaptability"},
        {name: "Responsibility"},
        {name: "Creativity"},
    ]
</script>

<div>
    <div id="blur"></div>
    <div class="header flex justify-evenly mt-28">
        <div class="flex flex-col">
            <h1 class="font-extrabold leading-10 tracking-tight sm:leading-none md:text-6xl text-4xl lg:text-7xl">Agustín <br> Dell' Aquila</h1>
            <p class="text-3xl mt-2">Fullstack Developer</p>
            <div class="flex mt-4">
                <a href="https://www.linkedin.com/in/agustin-dell-aquila-a5b2451b2/" target="_blank" rel="noreferrer">
                    <img class="w-12" src={LinkedIn} alt="LinkedIn"/>                    
                </a>
                <a href="https://github.com/agusdellaquila" target="_blank" rel="noreferrer">
                    <img class="w-12" src={Github} alt="Github"/>
                </a>
            </div>
        </div>
        <img class="logo hidden md:block lg:block" src={Logo} alt="Logo"/>
    </div>

    <div class="welcome flex justify-center">
        <div class="mt-16 lg:mt-32 flex flex-col items-center">
            <div class="flex font-extrabold leading-10 tracking-tight text-white text-center sm:leading-none md:text-6xl text-4xl lg:text-7xl">
                <div class="flex flex-col">
                    <p class="text-3xl md:text-4xl lg:text-6xl mt-4">WELCOME</p>
                    <img class="w-36" src={Underline} alt="Underline"/>
                </div>
                <div class="text-3xl md:text-4xl lg:text-6xl mt-4 ml-2">
                    <p>TO MY 
                        <a href="/personal">
                            <span class="bg-clip-text text-transparent bg-gradient-to-r from-orange-400 via-pink-400 to-violet-500">SPACE</span> 
                        </a>
                    </p>
                    <p class="text-left"> ON THE </p> 
                    <p class="text-left"> INTERNET</p>
                </div>
                <!-- <img class="ml-20 w-44 h-44" src={Paperplane} alt="Paperplane"/> -->
            </div>
        </div>
    </div>
    
    <img class="w-full" src={Clouds} alt="Clouds"/>

    <!-- WORK -->
    <div id="projects" class="welcome flex justify-center">
        <div class="flex flex-col mt-24 lg:mt-32 items-center">
            <p class="mt-4 font-extrabold leading-10 tracking-tight sm:leading-none md:text-6xl text-4xl lg:text-7xl">My best projects</p>

            <div class="projects mt-28">
                <img class="absolute w-24 -top-20 left-1/2 transform -translate-x-1/2" src={Crown} alt="Crown"/>
                <!-- <div class="grow"> -->
                    <a href="https://cobra-denim.vercel.app/" target="_blank" rel="noreferrer">
                        <img class="absolute bottom-80 left-0" src={Cobra} alt="Cobra Denim"/>
                    </a>
                <!-- </div> -->
                <!-- <div class="grow"> -->
                    <a href="/" target="_blank" rel="noreferrer">
                        <img class="absolute bottom-20 right-0" src={Stocksystem} alt="Stocksystem"/>
                    </a>
                <!-- </div> -->
                <!-- <a href="/" target="_blank" rel="noreferrer">
                    <img class="absolute bottom-60 left-0" src={Cobra} alt="Cobra Denim"/>
                </a>
                <a href="/" target="_blank" rel="noreferrer">
                    <img class="absolute bottom-40 right-0" src={Stocksystem} alt="Stocksystem"/>
                </a> -->
                <div class="grow">
                    <a href="https://binarybrainsdev.netlify.app/" target="_blank" rel="noreferrer">
                        <img class="absolute top-0 left-1/2 transform -translate-x-1/2" src={Binarybrains} alt="Binary Brains"/>
                    </a>
                </div>
            </div>
        </div>
    </div>

    <!-- SKILLS -->
    <div id="skills" class="welcome flex justify-center -mt-96">
        <div class="flex flex-col -mt-10 items-center">
            <h2 class="text-left font-extrabold leading-10 tracking-tight sm:leading-none md:text-6xl text-4xl lg:text-7xl">Skills</h2>

            <section class="skills mt-6">
                <h3 class="text-center text-2xl md:text-4xl lg:text-6xl font-bold">Programming & Design</h3>

                <div class="px-4 mt-8 flex flex-wrap justify-around gap-x-8 gap-y-4">
                    {#each skills as skill}
                        <Skill name={skill.name} icon={skill.icon} />
                    {/each}
                </div>

                <h3 class="text-center text-2xl md:text-4xl lg:text-6xl mt-10 font-bold">Soft Skills</h3>

                <div class="mt-8 px-4 flex flex-wrap justify-around gap-x-8 gap-y-4">
                    {#each softSkills as skill}
                        <Skill name={skill.name} icon={skill.icon} />
                    {/each}
                </div>
            </section>
        </div>
    </div>

    <!-- CONTACT -->
    <div id="contact" class="mt-16">
        <section>
            <div class="max-w-lg px-4 mx-auto text-left md:max-w-none md:text-center">
                 <h1 class="font-extrabold leading-10 tracking-tight text-white text-center sm:leading-none md:text-6xl text-4xl lg:text-7xl">
                   <span class=" mt-2 bg-clip-text text-transparent bg-gradient-to-r from-purple-400 via-emerald-400 to-lime-300 md:inline-block"> Contact me </span>
                 </h1>

                 <div class="flex mt-6 justify-center">
                    <a href="https://www.linkedin.com/in/agustin-dell-aquila-a5b2451b2/" target="_blank" rel="noreferrer">
                        <img class="w-12 grow" src={LinkedIn} alt="LinkedIn"/>                    
                    </a>
                    <a href="https://github.com/agusdellaquila" target="_blank" rel="noreferrer">
                        <img class="w-12 grow" src={Github} alt="Github"/>
                    </a>
                </div>  

                 <div class="mx-auto grow rounded-lg font-black mt-8 text-zinc-400 md:mt-12 md:max-w-lg text-center lg:text-lg">
                   <a href="mailto:agusdellaquila72@gmail.com" class="bg-tkb border font-medium text-sm text-white py-3 px-7 rounded-full">
                        Send an email 📬
                   </a>
                 </div>
                 <div class="mx-auto rounded-lg mt-8 md:mt-12 md:max-w-lg text-center lg:text-lg">
                        Or shedule a quick talk!
                  </div>
               </div>
        </section>
        <Calendly />
    </div>
    <!-- <Mouse /> -->
</div>