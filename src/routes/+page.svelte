<script lang="ts">
    let skills: { title: string; description: string; image: string; }[] = [
        {
            title: 'Build a website',
            description: 'From building fun websites for myself to creating complex systems for companies, I have the skills to create pretty much any site you could imagine.',
            image: 'lettersmith.png'
        },
        {
            title: 'Film & produce any video',
            description: 'My hobby of filming cars grew into a whole production company making marketing videos, music clips, car edits, or other videos & photos of any kind.',
            image: 'videoclip.png'
        },
        {
            title: 'Educate in IT',
            description: 'Since IT education in traditional schools is usually very poor, I decided to make fun workshops for children in elementary schools. I also teach teachers or whole companies.',
            image: 'educate.png'
        }
    ]
    let projects: { title: string; image: string; }[] = [
        {
            title: 'Luma production agency',
            image: 'luma.png'
        },
        {
            title: 'SX Media - car photos & videos',
            image: 'sxmedia.png'
        },
        {
            title: 'Lettersmith construction website',
            image: 'lettersmith.png'
        }
    ]
</script>

<main class="bg-[#181818] font-Montserrat text-white">
    <div class="flex w-full justify-center items-center pt-24 pb-6">
        <img src="/images/ksicht.png" alt="Avatar" class="w-48">
    </div>
    <h1 class="text-4xl font-bold text-center pb-4">Hi, I'm Oliver</h1>
    <h3 class="text-center text-white text-opacity-80 text-lg px-10 font-light">A passionate cybersecurity student from Prague</h3>
    <h1 class="text-3xl font-semibold text-center pt-20 pb-6 text-white text-opacity-90">What can I do?</h1>
    <section class="w-full flex flex-col justify-center px-10 gap-14">
        {#each skills as skill}
            <div class="flex flex-col gap-2">
                <img src="images/{skill.image}" alt="Web development" class="w-full rounded-md">
                <h2 class="font-bold text-lg mt-2">{skill.title}</h2>
                <p class="text-white text-opacity-75 pb-1">{skill.description}</p>
                <button class="font-semibold bg-white text-[#181818] rounded-md px-4 py-1.5">Find out more</button>
            </div>
        {/each}
    </section>
    <h1 class="text-3xl font-semibold text-center pt-16 pb-6 text-white text-opacity-90">My projects</h1>
    <section class="w-full flex flex-col justify-center px-5 gap-14">
        {#each skills as skill}
            <div class="flex flex-col gap-2">
                <img src="images/{skill.image}" alt="Web development" class="w-full rounded-md">
                <h2 class="font-bold text-lg mt-2">{skill.title}</h2>
                <p class="text-white text-opacity-75 pb-1">{skill.description}</p>
                <button class="font-semibold bg-white text-[#181818] rounded-md px-4 py-1.5">Find out more</button>
            </div>
        {/each}
    </section>
    <h6 class="pb-6 pt-16 text-center">© 2025 Oliver Cingl</h6>
</main>