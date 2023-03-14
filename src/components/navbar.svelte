<script>
    import Logo from '../assets/Landing/logo.png';
</script>

<div class="flex flex-col items-center justify-center" x-cloak x-data="appData()" x-init="appInit()">
    <div class="flex flex-col font-extrabold leading-10 tracking-tight sm:leading-none">
        <!-- Navbar -->
        <nav class="flex justify-around py-4 backdrop-blur-md w-full fixed top-0 left-0 right-0 z-10 font-semibold">

            <!-- Logo Container -->
            <div class="flex items-center">
                <!-- Logo -->
                <a href="/" class="cursor-pointer">
                    <img class="h-10 object-cover grow" src={Logo} alt="Logo">
                </a>
            </div>

            <!-- Links Section -->
            <div class="items-center hidden space-x-8 lg:flex">
                <a href="/" class="flex hover:text-indigo-200 cursor-pointer transition-colors duration-300">
                    Home
                </a>

                <a href=/#projects class="flex cursor-pointer transition-colors duration-300 font-semibold">
                    Projects
                </a>

                <a href=/#skills class="flex hover:text-indigo-200 cursor-pointer transition-colors duration-300">
                    Skills
                </a>

                <a href="/personal" class="flex hover:text-indigo-200 cursor-pointer transition-colors duration-300">
                    Personal
                </a>

                <a href="/about" class="flex hover:text-indigo-200 cursor-pointer transition-colors duration-300">
                    About me
                </a>
            </div>

            <!-- Icon Menu Section -->
            <div class="flex items-center space-x-5">
                <a href="https://drive.google.com/file/d/1tffflNdZPUoz8NpNNY8hdFTp8xSr-JQS/view?usp=share_link" target="_blank" rel="noreferrer" class="flex hover:text-indigo-200 cursor-pointer transition-colors duration-300">
                    Download CV
                </a>

                <a href=/#contact class="flex hover:text-indigo-200 cursor-pointer transition-colors duration-300">  
                    Contact
                </a>
            </div>
        </nav>
    </div>
</div>