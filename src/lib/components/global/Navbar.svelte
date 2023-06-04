<script lang="ts">
    import Logo from "./Logo.svelte";
    import { Database, LineChart, Wrench } from "lucide-svelte";
    import Button from "$components/ui/button/Button.svelte";
    import Avatar from "$components/ui/avatar/Avatar.svelte";
    import AvatarImage from "$components/ui/avatar/AvatarImage.svelte";
</script>

<aside class="sticky w-20 flex flex-col items-center border-r h-screen bg-white p-5">
    <div>
        <!--Logo-->
        <Logo />
    </div>

    <ul class="mt-9 flex flex-col gap-5">
        <li>
            <Button variant="outline" class="px-2 border-black border-2 rounded-lg">
                <Database class="w-6 h-6" />
            </Button>
        </li>

        <li>
            <!--TODO: Variant is outline if it is the ACTIVE PAGE!-->
            <Button variant="ghost" class="p-2 rounded-xl">
                <LineChart class="w-6 h-6" />
            </Button>
        </li>

        <li>
            <Button variant="ghost" class="p-2 rounded-xl">
                <Wrench class="w-6 h-6" />
            </Button>
        </li>
    </ul>

    <div class="mt-auto">
        <!--Logout Button/Avatar-->
        <Avatar>
            <AvatarImage src="https://github.com/shadcn.png" alt="@shadcn" />
        </Avatar>
    </div>
</aside>