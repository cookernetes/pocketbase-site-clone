<script lang="ts">
    import { Input } from "./ui/input";
    import Button from "$components/ui/button/Button.svelte";
    import { Users, Folder, LayoutDashboard } from "lucide-svelte";
</script>

<aside class="sticky h-screen w-48 border-r">
    <div class="border-b w-full px-2.5 py-6">
        <Input type="text" placeholder="Search collections" class="border-0" />
    </div>

    <div class="px-2.5 mt-4">
        <ul class="flex flex-col gap-2.5">
            <li>
                <!--SECONDARY VARIANT IS FOR ACTIVE BUTTONS!-->
                <Button variant="secondary" class="gap-2.5 w-full justify-start px-2">
                    <Users class="h-5" /> users
                </Button>
            </li>

            <li>
                <Button variant="ghost" class="gap-2.5 w-full justify-start px-2 text-muted-foreground">
                    <Folder class="h-5" /> messages
                </Button>
            </li>

            <li>
                <Button variant="ghost" class="gap-2.5 w-full justify-start px-2 text-muted-foreground">
                    <Folder class="h-5" /> posts
                </Button>
            </li>

            <li>
                <Button variant="ghost" class="gap-2.5 w-full justify-start px-2 text-muted-foreground">
                    <LayoutDashboard class="h-5" /> messagesReport
                </Button>
            </li>

            <li class="mt-2.5">
                <Button variant="outline" class="border-2 border-black rounded-sm w-full">
                    <span class="pr-2">+</span> New collection
                </Button>
            </li>
        </ul>
    </div>
</aside>