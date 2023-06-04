<script>
    import Breadcrumbs from "$components/global/Breadcrumbs.svelte";
    import { Settings, RefreshCcw, Webhook } from "lucide-svelte";
    import Button from "$components/ui/button/Button.svelte";
</script>

<main class="bg-slate-100 w-full p-8">
    <div class="flex items-center">
        <Breadcrumbs />

        <div class="flex ml-6 gap-3">
            <Button variant="ghost" class="rounded-full px-2">
                <Settings class="w-5 h-5" />
            </Button>

            <Button variant="ghost" class="rounded-full px-2">
                <RefreshCcw class="w-5 h-5" />
            </Button>
        </div>
    </div>

    <div class="w-full mt-4">
        <div class="w-full flex items-center gap-2">
            <Button variant="outline" class="w-1/2 border-2 border-black rounded-sm">
                 <Webhook class="w-4 h-4 mr-2" /> API Preview
            </Button>

            <Button class="w-1/2 items-center">
                <span class="pr-2 text-xl font-light">+</span> New record
            </Button>
        </div>
    </div>
</main>