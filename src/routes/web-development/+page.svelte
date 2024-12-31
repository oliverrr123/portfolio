<script lang="ts">
    let websites: { title: string; description: string; image: string; link: string; }[] = [
        {
            title: 'Lettersmith construction company',
            description: 'A portfolio site for a London construction company - Comas Lettersmith Ltd including a couple images and an e-mail contact form.',
            image: 'lettersmith.png',
            link: 'https://comaslettersmith.co.uk/'
        },
        {
            title: 'Luma production',
            description: 'Another portfolio website, this time for my media production company - Luma production. It’s a simple one-pager including all the necessary info.',
            image: 'luma.png',
            link: 'https://luma-production.com/'
        },
        {
            title: 'SX Media',
            description: 'A showcase site of my work in documenting cars. Including a gallery with my best pics.',
            image: 'sxmedia.png',
            link: 'https://sx-media.vercel.app/'
        }
    ]
    let tools: { name: string; image: string; }[] = [
        {
            name: 'HTML',
            image: 'html.svg'
        },
        {
            name: 'CSS',
            image: 'css.svg'
        },
        {
            name: 'JavaScript',
            image: 'javascript.svg'
        },
        {
            name: 'Svelte',
            image: 'svelte.svg'
        },
        {
            name: 'Tailwind',
            image: 'tailwind.svg'
        },
        // {
        //     name: 'Tailwind CSS',
        //     image: 'tailwind.svg'
        // },
        // {
        //     name: 'Vercel',
        //     image: 'vercel.svg'
        // }
        {
            name: 'Prisma',
            image: 'prisma.svg'
        },
        {
            name: 'PostgreSQL',
            image: 'postgres.svg'
        },
        {
            name: 'Python',
            image: 'python.svg'
        },
        {
            name: 'GitHub',
            image: 'github.svg'
        },
    ]
</script>

<main class="bg-[#181818] font-Montserrat text-white px-10">
    <a href="/" class="text-white text-sm text-opacity-50 underline pt-16 block">{'<'}&nbsp; Back to main page</a>
    <h1 class="text-3xl font-bold pb-8 pt-2">Web development</h1>
    <h3 class="text-white text-opacity-80 text-lg font-light">Over the years, I've honed my skills in creating websites that are not only visually stunning but also functional and optimized for various needs. Whether it's a personal blog, a professional portfolio, or a complex e-commerce platform, I bring creativity and technical expertise to every project.</h3>
    <h2 class="text-xl font-semibold pt-20 pb-6 text-white text-opacity-90">Websites I built:</h2>
    <section class="w-full flex flex-col justify-center gap-14">
        {#each websites as website}
            <div class="flex flex-col gap-2">
                <img src="/images/{website.image}" alt="Web development" class="w-full rounded-md">
                <h2 class="font-bold text-lg mt-2">{website.title}</h2>
                <p class="text-white text-opacity-75 pb-1">{website.description}</p>
                <a href={website.link}><button class="font-semibold bg-white text-[#181818] rounded-md px-4 py-1.5">Find out more</button></a>
            </div>
        {/each}
    </section>
    <h2 class="text-2xl font-semibold pt-20 pb-6 text-white text-opacity-90">Tools I use:</h2>
    {#each tools as tool}
        <div class="flex gap-1 items-center">
            <img src="/icons/web-development/{tool.image}" alt="{tool.name}" class="w-12 h-12 p-2">
            <p>{tool.name}</p>
        </div>
    {/each}
    <div class="flex justify-center gap-4 pt-16">
        <a href="https://github.com/oliverrr123/" target="_blank"><img src="/icons/github.svg" alt="GitHub" class="w-8 h-8 opacity-75 hover:opacity-100 transition-opacity"></a>
        <a href="https://linkedin.com/in/olivercingl/" target="_blank"><img src="/icons/linkedin.svg" alt="LinkedIn" class="w-8 h-8 opacity-75 hover:opacity-100 transition-opacity"></a>
        <a href="mailto:oliver.cingl@gmail.com" target="_blank"><img src="/icons/mail.svg" alt="Mail" class="w-8 h-8 opacity-75 hover:opacity-100 transition-opacity"></a>
    </div>
    <h6 class="py-6 text-center">© 2025 Oliver Cingl</h6>
</main>