<template>
    <div class="bg-gray-50 text-gray-800 min-h-screen flex flex-col">
        <header class="border-b border-gray-500/50 h-[68px] flex">
            <PageContainer class="flex-1 flex items-center">
                <div>Ophams</div>
            </PageContainer>
        </header>
        <main class="flex-1 flex">
            <slot />
        </main>
        <footer class="border-t border-gray-500/50 h-[38px] flex">
            <PageContainer class="flex-1 flex items-center">
                <div class="flex-1 text-center">
                    <span>&copy; 2024</span>
                </div>
            </PageContainer>
        </footer>
    </div>
</template>