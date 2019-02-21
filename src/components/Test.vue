<template>
    <div id="Head">
      <p>Welcome <b>{{ name }}</b></p>
        <div id=hbody>
            <p>Skill Set</p>
           <form @submit.prevent="addSkill">
               <input type="text" placeholder="Enter skill" v-model="skill">
            </form>
            <ul id="Test">
                <li v-for="(data, index) in skills" :key='index'>
                    {{ data.skill }}
                </li>
            </ul>
        </div>
    </div>
</template>

<script>
export default {
    name : 'Test',
    data () {
        return {
            skill: '',
            skills : [{
                skill : 'Frontend Developer',
                rating :  '8.0'
            },
            {
                skill : 'Backend Developer',
                rating :  '9.0'
            }],
            name : 'Fritz'
        }
    },
    methods : {
        addSkill() {
            this.skills.push({skill : this.skill})
            this.skill = '';
        }
    }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Montserrat');
    body {
        background-color: #eeeeee;
    }
    #Head{
        font-family: 'Montserrat', 'san-serif';
        font-size: 20pt
    }
    #hbody{
        font-size: 12pt;
        display: grid;
    }
    ul{
        list-style-position: inside;
    }
    li{
        padding: 10px;
        text-decoration: none; 
        background: #ffffff;
        border-radius: 2px;
        color : blue;
        font-weight: bold;
        margin-top: 15px;
        
    }
    #nav a{
        float: left
    }
</style>
