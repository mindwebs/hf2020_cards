---
title: Ayushman Bilas Thakur
institution: Kalyani Government Engineering College
interests: [Fullstack Web Development]
layout: blog
---

## Hello,

Ayushman Bilas Thakur here. Thanks for looking at my page. 

My page is basically here to make you aware about what you can do in this page. Here you can do anything! These markdown pages are powered by Vue JS. So you can do things like this:

<div class="vue-zone"> 
    You have clicked the button below for <strong>{{count}}</strong> times. 
    <button @click="clicked()">Click me!</button>
    <p>Yes you can override styles and can also implement Javascript with vue.js</p>
</div>

So opportunity with this repo is endless!

<script>
    export default {
        data(){
            return(
                {
                    count: 0
                }
            )
        },
        methods: {
            clicked: function(){
                this.count++
            }
        }
    }
</script>


<style scoped>
    .vue-zone{
        padding: 20px;
        background: #eee;
        box-shadow: 5px 5px 10px 0px rgba(0,0,0,0.5);
    }
</style>