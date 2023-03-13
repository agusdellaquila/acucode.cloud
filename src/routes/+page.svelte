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
    import Hexa from '../assets/Landing/hexa.png';
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
        {name: "Organization and time management"},
        {name: "Attention to detail"},
        {name: "Punctuality"},
        {name: "Adaptability"},
        {name: "Responsibility"},
        {name: "Creativity"},
    ]
</script>

<div>
    <div id="blur"></div>
    <div class="header flex justify-evenly mt-40">
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
        <img class="logo" src={Logo} alt="Logo"/>
    </div>

    <div class="welcome flex justify-center">
        <div class="flex flex-col mt-44 items-center">
            <div class="flex font-extrabold leading-10 tracking-tight text-white text-center sm:leading-none md:text-6xl text-4xl lg:text-7xl">
                <div class="flex flex-col">
                    <p class="text-6xl mt-4">WELCOME</p>
                    <img class="w-72" src={Underline} alt="Underline"/>
                </div>
                <p class="text-6xl mt-4 ml-6">TO MY  
                    <span class="bg-clip-text text-transparent bg-gradient-to-r from-orange-400 via-pink-400 to-violet-500 md:inline-block">SPACE</span> 
                    <br> ON THE <br> INTERNET</p>
                <!-- <img class="ml-20 w-44 h-44" src={Paperplane} alt="Paperplane"/> -->
            </div>
            <img src={Clouds} alt="Clouds"/>
        </div>
    </div>

    <!-- WORK -->
    <div class="welcome flex justify-center">
        <div class="flex flex-col mt-44 items-center">
            <p class="mt-4 font-extrabold leading-10 tracking-tight sm:leading-none md:text-6xl text-4xl lg:text-7xl">My best projects</p>

            <div class="relative">
                <img class="absolute bottom-60 left-0" src={Cobra} alt="Cobra Denim"/>
                <img class="absolute top-0 left-1/2 transform -translate-x-1/2 z-10" src={Binarybrains} alt="Binary Brains"/>
                <img class="absolute bottom-40 right-0" src={Hexa} alt="Hexa"/>
            </div>
        </div>
    </div>

    <!-- SKILLS -->
    <div class="welcome flex justify-center">
        <div class="flex flex-col mt-44 items-center">
            <h2 class="mt-4 text-left font-extrabold leading-10 tracking-tight sm:leading-none md:text-6xl text-4xl lg:text-7xl">Skills</h2>

            <section class="skills mt-20">
                <h3 class="text-4xl">Programming & Design</h3>

                <div class="mt-8 flex flex-wrap gap-x-8 gap-y-4">
                    {#each skills as skill}
                        <Skill name={skill.name} icon={skill.icon} />
                    {/each}
                </div>

                <h3 class="text-4xl mt-20">Soft Skills</h3>

                <div class="mt-8 flex flex-wrap gap-x-8 gap-y-4">
                    {#each softSkills as skill}
                        <Skill name={skill.name} icon={skill.icon} />
                    {/each}
                </div>
            </section>
        </div>
    </div>

    <!-- CONTACT -->
    <div class="mt-40">
        <p class="text-center mt-4 font-extrabold leading-10 tracking-tight sm:leading-none md:text-6xl text-4xl lg:text-7xl">CONTACT</p>

        <p class="text-center mt-14 font-semibold leading-10 tracking-tight sm:leading-none text-lg">Shedule a quick talk!</p>
        <Calendly />
    </div>
    <!-- <Mouse /> -->
</div>