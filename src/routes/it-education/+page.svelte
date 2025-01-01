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
            name: 'TypeScript',
            image: 'typescript.svg'
        },
        {
            name: 'Svelte',
            image: 'svelte.svg'
        },
        {
            name: 'Tailwind',
            image: 'tailwind.svg'
        },
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

<a href="/" class="text-white text-sm text-opacity-50 underline pt-16 block">{'<'}&nbsp; Back to main page</a>
<h1 class="text-3xl font-bold pb-8 pt-2">IT Education</h1>
<h3 class="text-white text-opacity-80 text-lg font-light pb-16">I made a couple workshops for kids in elementary schools. Teachers also liked them, so I made workshops for them separately. Now, I’m continuing doing more, even for company employees or individuals.</h3>
<img src="/images/educate.png" alt="Web development" class="w-full">