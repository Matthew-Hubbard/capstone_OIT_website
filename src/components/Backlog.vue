<template>
    <div class="backlog">
        <h1>Product Backlog</h1>
<!--        <div class="holder">-->
            <table>
                <tr>
                    <th>Front-end</th>
<!--                    <th>Status</th>-->
                    <th>Back-end</th>
<!--                    <th>Status</th>-->
                </tr>
                <tr>
                    <td>
                        <ul>
                            <li v-for="(data, index) in frontEnd" :key="index">{{ data.task }} - ({{ data.status }})</li>
                        </ul>
                    </td>

<!--                    <td>-->
<!--                        <p v-for="(data, index) in frontEnd" :key="index">{{ data.status }}</p>-->
<!--                    </td>-->

                    <td>
                        <ul>
                            <li v-for="(data, index) in backEnd" :key="index">{{ data.task }} - ({{ data.status }})</li>
                        </ul>
                    </td>

<!--                    <td>-->
<!--                        <p v-for="(data, index) in backEnd" :key="index">{{ data.status }}</p>-->
<!--                    </td>-->
                </tr>
            </table>
        </div>
<!--    </div>-->
</template>

<script>
    export default {
        name: "Backlog",
        data() {
            return {
                frontEnd: [
                    { "task": "Wireframe Design", "status": "In Progress" },
                    { "task": "Login Page", "status": "Done" },
                    { "task": "Remove Vue Default Junk", "status": "In Progress" },
                    { "task": "Input Sanitization", "status": "Todo" },
                    { "task": "PSU Alerts Display", "status": "Final Touches/Review" },
                    { "task": "PSU Alerts Input Fields", "status": "Final Touches/Review" },
                    { "task": "Emergency Contact Display", "status": "Todo" },
                    { "task": "Emergency Contact Input Interface", "status": "Todo" },
                    { "task": "Evacuation Assistance Display and Checkbox", "status": "In Progress" },
                    { "task": "Inactivity Timeout", "status": "Todo" },
                    { "task": "Home and Logout Buttons", "status": "Todo" },
                    { "task": "Success/Failure Message on Form Completion", "status": "Todo" },
                    { "task": "Sticky Navbar Prototype", "status": "Todo" },
                    { "task": "Expandable/Collapsible Text Prototype", "status": "Todo" },
                    { "task": "Side Navigation Prototype", "status": "Todo" },
                ],
                backEnd: [
                    { "task": "Input Sanitization", "status": "In Progress"},
                    { "task": "Login JWT Authentication", "status": "In Progress"},
                    { "task": "Evac Assistance Send Status", "status": "In Progress"},
                    { "task": "Evac Assistance Update Status", "status": "In Progress"},
                    { "task": "PSU Alert Send Info", "status": "Todo"},
                    { "task": "PSU Alert Update Info", "status": "Todo"},
                    { "task": "Emergency Contacts Send Contacts", "status": "Todo"},
                    { "task": "Emergency Contacts Update Contacts", "status": "Todo"},
                    { "task": "Update Activity Times", "status": "Todo"},
                ]
            }
        }
    }
</script>

<style scoped>

ul {
  /*list-style-type: square;*/
  padding: 0;
}

li {
    /*display: inline-block;*/
    margin: 0 30px;
}

a {
  color: #42b983;
}


h3{
    text-align: center;
}

table{
    border: 1px solid black;
    width: 50%;
    position: fixed;
    left: 50%;
    margin-left: -25%; /*half of the width*/
}

th{
    border: 1px solid black;
    text-align: center;
}

td {
    border: 1px solid black;
    text-align: left;
    vertical-align: top;
}

/*.holder{*/
/*    border-style: dashed;*/
/*    border-width: thin;*/
/*    text-align: left;*/
/*    width: 40%;*/
/*    position: fixed;*/
/*    left: 50%;*/
/*    margin-left: -20%;*/
/*}*/
</style>