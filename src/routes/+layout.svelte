<script>
    import "../app.css";
    import { injectAnalytics } from '@vercel/analytics/sveltekit'

    let { children } = $props();
</script>

<main class="bg-[#181818] font-Montserrat text-white px-10 sm:px-[15vw] md:px-[20vw] lg:px-[25vw] xl:px-[33vw]">
    {@render children()}
    <footer>
        <div class="flex justify-center gap-4 pt-16">
            <a href="https://github.com/oliverrr123/" target="_blank" aria-label="Github profile"><img src="/icons/github.svg" alt="Link to my GitHub" class="w-8 h-8 opacity-75 hover:opacity-100 transition-opacity"></a>
            <a href="https://linkedin.com/in/olivercingl/" target="_blank" aria-label="Linkedin profile"><img src="/icons/linkedin.svg" alt="Link to my LinkedIn" class="w-8 h-8 opacity-75 hover:opacity-100 transition-opacity"></a>
            <a href="mailto:oliver.cingl@gmail.com" target="_blank" aria-label="Email"><img src="/icons/mail.svg" alt="Link to my email" class="w-8 h-8 opacity-75 hover:opacity-100 transition-opacity"></a>
        </div>
        <h6 class="py-6 text-center">© 2025 Oliver Cingl</h6>
    </footer>
</main>