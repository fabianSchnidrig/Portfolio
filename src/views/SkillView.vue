<template>
    <section class="skills">
        <h1 class="title">My Skills</h1>

        <div class="skill">
            <span>Vue.js</span>
            <div class="bar">
                <div style="width: 85%"></div>
            </div>
        </div>

        <div class="skill">
            <span>JavaScript</span>
            <div class="bar">
                <div style="width: 80%"></div>
            </div>
        </div>

        <div class="skill">
            <span>Docker</span>
            <div class="bar">
                <div style="width: 70%"></div>
            </div>
        </div>

        <div class="skill">
            <span>Linux Server</span>
            <div class="bar">
                <div style="width: 90%"></div>
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: "SkillView",
};
</script>

<style scoped>
.skills {
    min-height: 100vh;
    padding: 80px 10%;
    background: #0a0a0a;
    color: white;
}

.title {
    font-size: 42px;
    margin-bottom: 40px;
    color: #00bcd4;
}

.skill {
    margin-bottom: 25px;
}

.skill span {
    font-size: 20px;
}

.bar {
    width: 100%;
    height: 12px;
    background: #222;
    border-radius: 6px;
    margin-top: 8px;
}

.bar div {
    height: 100%;
    background: #00bcd4;
    border-radius: 6px;
}
</style>
