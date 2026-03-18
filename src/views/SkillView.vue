<template>
    <section class="skills">
        <h1 class="title">My <span>Skills</span></h1>

        <div class="skill">
            <div class="skill-header">
                <span>Vue.js</span>
                <span>55%</span>
            </div>
            <div class="bar">
                <div style="width: 55%"></div>
            </div>
        </div>

        <div class="skill">
            <div class="skill-header">
                <span>JavaScript</span>
                <span>65%</span>
            </div>
            <div class="bar">
                <div style="width: 65%"></div>
            </div>
        </div>
        <div class="skill">
            <div class="skill-header">
                <span>HTML & CSS</span>
                <span>50%</span>
            </div>
            <div class="bar">
                <div style="width: 50%"></div>
            </div>
        </div>
        <div class="skill">
            <div class="skill-header">
                <span>Linux Server Administration</span>
                <span>70%</span>
            </div>
            <div class="bar">
                <div style="width: 70%"></div>
            </div>
        </div>


<div class="skill">
            <div class="skill-header">
                <span>Docker</span>
                <span>75%</span>
            </div>
            <div class="bar">
                <div style="width: 75%"></div>
            </div>
        </div>

        <div class="skill">
            <div class="skill-header">
                <span>Networking Basics</span>
                <span>60%</span>
            </div>
            <div class="bar">
                <div style="width: 60%"></div>
            </div>
        </div>


        <div class="skill">
            <div class="skill-header">
                <span>SSH Remote Access</span>
                <span>60%</span>
            </div>
            <div class="bar">
                <div style="width: 60%"></div>
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
    height: 10px;
    background: #1a1a1a;
    border-radius: 6px;
    margin-top: 8px;
    overflow: hidden;
}

.bar div {
    height: 100%;
    background: linear-gradient(90deg, #00bcd4, #00d4ee);
    border-radius: 6px;
}

.title span {
    color: #00bcd4;
}

.skill-header {
    display: flex;
    justify-content: space-between;
    font-size: 18px;
}
</style>
