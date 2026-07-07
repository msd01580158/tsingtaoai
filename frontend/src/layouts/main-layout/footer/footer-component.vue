<template>
    <div class="text-placeholder">
        <q-toolbar>
            <q-toolbar
                class="flex text-center justify-between"
                style="font-size: 12px"
            >
                <div class="flex" style="gap: 8px">
                    <span>
                        © {{ year }} TsingtaoAI - 机器人系统实验室 (RSL)
                    </span>
                    <footer-separator />
                    <footer-build-info />
                </div>
                <footer-status-page-link />
            </q-toolbar>
        </q-toolbar>
    </div>
</template>

<script setup lang="ts">
import FooterBuildInfo from './footer-build-info.vue';
import FooterSeparator from './footer-separator.vue';
import FooterStatusPageLink from './footer-status-page-link.vue';

const year = new Date().getFullYear();
</script>
