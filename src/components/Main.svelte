<script>
    import Step from "./Step.svelte";

    let steps = [
        {
            name: "MBBS",
            icon: "fa-solid fa-hospital",
            description:
                "MBBS is an undergraduate degree in the field of medicine. It equips students with foundational knowledge and skills necessary for clinical practice. Throughout the program, I studied various medical disciplines, including anatomy, physiology, pathology, pharmacology, and clinical medicine. This degree forms the basis for further specialization and training in specific areas of medicine, such as cardiology.",
        },
        {
            name: "MCPS",
            icon: "fa-solid fa-stethoscope",
            description:
                "MCPS is a postgraduate medical qualification that indicates a level of expertise in a particular medical specialty. It is awarded by the College of Physicians and Surgeons, demonstrating proficiency in clinical skills and knowledge relevant to the chosen specialty.",
        },
        {
            name: "DABIM (USA)",
            icon: "fa-solid fa-house-medical",
            description:
                "DABIM certification is granted by the American Board of Internal Medicine to physicians who have completed rigorous training and demonstrated expertise in internal medicine. It signifies proficiency in diagnosing, treating, and managing various medical conditions, including those related to the cardiovascular system. ",
        },
        {
            name: "DABG (USA)",
            icon: "fa-solid fa-book",
            description:
                "DABG certification is awarded by the American Board of Geriatrics to physicians specializing in geriatric medicine. It indicates proficiency in addressing the unique healthcare needs of older adults, including the diagnosis, treatment, and prevention of age-related conditions, such as cardiovascular diseases.",
        },

    ];

    let benefits = [
        {
            metric: "10x",
            name: "a Consultant Physician",
            description:
                "I bring a fusion of expertise, passion, and dedication to the realm of healthcare. I strive to provide precise diagnoses and comprehensive care to individuals with diverse cardiac conditions. My expertise extends to areas such as cardiac rehabilitation and exercise, where I work tirelessly to enhance the cardiovascular health and well-being of my patients.",
        },
        {
            name: "a Geriatrician",
            description:
                "Beyond clinical practice, I am driven by a profound passion for fostering meaningful patient experiences and promoting holistic well-being. I firmly believe that effective healthcare goes beyond treating symptoms; it involves understanding the unique needs and aspirations of each individual under my care.",
        },
        {
            name: "an excellent communicator",
            description:
                "My approach is characterized by open communication, transparency, and a collaborative spirit. I prioritize building trusting relationships with my patients, empowering them to actively participate in their healthcare journey and make informed decisions. With a commitment to lifelong learning and innovation, I continually seek to stay abreast of the latest advancements in my field. Whether it's exploring new diagnostic techniques or embracing emerging therapies, I am dedicated to delivering the highest standard of care to those I serve. In essence, I am not just a physician; I am a compassionate advocate for the health and well-being of my patients, striving to make a positive impact on their lives each day.",
        },
    ];

    function scrollToFooter() {
        const footer = document.getElementById('getintouch');
        footer.scrollIntoView({ behavior: 'smooth' });
    }

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
                Hi! I'm <span class="poppins text-violet-400">Munir</span> H. <span class="poppins text-violet-400">Faswala</span>
                <br /> Consultant Physician & 
                <span class="poppins text-violet-400">Geriatrician</span>
            </h2>
            <p class="text-base sm:text-lg md:text-xl">
                My <span class="text-violet-400"> areas of expertise</span> includes Cardiac Imaging – Non-invasive, Cardiac Rehabilitation and Exercise, Hypertrophic Cardiomyopathy, Inherited Heart Diseases. 
            </p>
            <button
                class="blueShadow mx-auto lg:mr-auto lg:ml-0 text-base sm:text-lg md:text-xl poppins relative overflow-hidden px-6 py-3 group rounded-full bg-white text-slate-950"
                on:click={scrollToFooter}
            >
                <div
                    class="absolute top-0 right-full w-full h-full bg-violet-400 opacity-20 group-hover:translate-x-full z-0 duration-200"
                />
                <h4 class="relative z-9">Get in touch &rarr;</h4>
            </button>
        </div>
        <div class="relative shadow-2xl grid place-items-center">
            <img
                src={"images/1.jpg"}
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
            href="https://youtu.be/fZa6WcgcmE4?si=arVLigvvu3TQP0qP"
            target="_blank"
            class="mx-auto px-4 py-2 rounded-md border border-solid border-white flex items-center gap-2 -mb-4 sm:-mb-0 -mt-10 hover:border-violet-700 duration-200"
        >
            <i class="fa-regular fa-circle-play" />
            <p>Watch the video</p>
        </a>
        <div class="grid grid-cols-1 lg:grid-cols-4 gap-12 lg:gap-10">
            <Step step={steps[0]}>
            <p>
            <strong class="text-violet-400">MBBS</strong> is an undergraduate degree in the field of medicine.
             It equips students with foundational knowledge and skills necessary for clinical practice. Throughout the program, I studied various medical disciplines, including <strong class="text-violet-400">anatomy, physiology, pathology, pharmacology, and clinical medicine</strong>."
            </p> 
            </Step>
            <Step step={steps[1]}>
                <p>
                <strong class="text-violet-400">MCPS</strong> is a postgraduate medical qualification that indicates a level of expertise in a particular medical specialty. It is awarded by the <strong class="text-violet-400">College of Physicians and Surgeons</strong>, demonstrating proficiency in clinical skills and knowledge.
                </p>
            </Step>
            <Step step={steps[2]}>
                <p>
                <strong class="text-violet-400">DABIM</strong> certification is granted by the <strong class="text-violet-400"> American Board of Internal Medicine</strong> to physicians who have completed rigorous training and demonstrated expertise in <strong class="text-violet-400">internal medicine</strong>. 
                It signifies proficiency in diagnosing, treating, and managing various medical conditions, including those related to the cardiovascular system. 
                </p>
            </Step>
            <Step step={steps[3]}>
                <p>
                <strong class="text-violet-400">DABG</strong> certification is awarded by the <strong class="text-violet-400"> American Board of Geriatrics</strong> to physicians specializing in <strong class="text-violet-400">geriatric medicine</strong>. 
                It indicates proficiency in addressing the unique healthcare needs of older adults, including the diagnosis, treatment, and prevention of age-related conditions, such as <strong class="text-violet-400">cardiovascular diseases</strong>.
                </p>
            </Step>
        </div>
    </section>
    <section id="about" class="py-20 pt-10 lg:pt-16 lg:py-32 flex flex-col gap-16 sm:gap-20 md:gap-24 relative">
        <!-- <div class="z-[-1] bg-violet-950 w-screen left-1/2 -translate-x-1/2 top-0 h-full absolute"> </div> -->
        <div class="flex flex-col gap-2 text-center relative before:absolute before:top-0 before:left-0 before:w-2/3 before:h-1.5 before:bg-violet-700 after:absolute after:bottom-0 after:right-0 after:w-2/3 after:h-1.5 after:bg-violet-700 py-4">
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
            </section>
</main>
