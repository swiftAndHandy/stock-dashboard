<template>
    <BaseCard>
        <div class="corp-card">
            <div class="corp-header">
                <img src="" alt="logo">
                <span>{{ corpName }}</span>
            </div>
            <div class="corp-body">
                <span>Revenue Q1 2024</span>
                <article class="numbers">
                    <div class="numbers__primary">
                        {{ primaryNumber }}
                    </div>
                    <div class="numbers__secondary">
                        <div class="numbers__changes">
                            <span class="numbers__value">{{ absoluteChange }}</span>&nbsp;
                            <img src="" alt="+">
                        </div>
                        <div class="numbers__changes">
                            <span class="numbers__value">{{ relativeChange }}</span>&nbsp;
                            <span>%</span>
                        </div>
                    </div>
                </article>
                <span>In Bill USD</span>
            </div>
        </div>
    </BaseCard>
</template>

<script>
import BaseCard from './BaseCard.vue';

export default {
    name: 'CorpCard',
    components: {
        BaseCard
    },
    props: {
        corpName: {
            type: String,
            required: true
        },
        primaryNumber: {
            type: Number,
            default: 30 // Default-Wert festlegen
        },
        absoluteChange: {
            type: Number,
            default: 0
        },
        relativeChange: {
            type: Number,
            default: 0
        }
    },
}
</script>

<style scoped>
.corp-header {
    font-family: 'Rubik', Arial, Helvetica, sans-serif;
    font-weight: 500;
    font-size: 20px;
}

.corp-body {
    display: flex;
    flex-direction: column;
    gap: 4px;
}

.numbers {
    display: flex;
    align-items: center;
    gap: 4px;
    font-weight: 500;
}

.numbers__primary {
    font-size: 24px;
}

.numbers__secondary {
    display: flex;
    flex-direction: column;
    flex: 1;
}

.numbers__changes {
    display: flex;
    flex: 1;
}

.numbers__value {
    flex: 1;
    text-align: right
}
</style>