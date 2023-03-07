<template>
  <main>
<section>
  <div  class=" flex flex-row justify-between p-7 bg-gradient-to-r from-gray-700 to-cyan-900">
    <!---LOGO--->
    <div class=" flex flex-row">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M4.26 10.147a60.436 60.436 0 00-.491 6.347A48.627 48.627 0 0112 20.904a48.627 48.627 0 018.232-4.41 60.46 60.46 0 00-.491-6.347m-15.482 0a50.57 50.57 0 00-2.658-.813A59.905 59.905 0 0112 3.493a59.902 59.902 0 0110.399 5.84c-.896.248-1.783.52-2.658.814m-15.482 0A50.697 50.697 0 0112 13.489a50.702 50.702 0 017.74-3.342M6.75 15a.75.75 0 100-1.5.75.75 0 000 1.5zm0 0v-3.675A55.378 55.378 0 0112 8.443m-7.007 11.55A5.981 5.981 0 006.75 15.75v-1.5" />
</svg>
      <h1>SHELBY</h1>
    </div>
    <!---NAVBAR--->
    <div class=" flex flex-row gap-8 pl-80 text-lg">
    <div class=" flex flex-row ">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
</svg>
      <nav class=" flex flex-row gap-5">
           <router-link to="/">Home</router-link>
      </nav>
    </div>
    <div class=" flex flex-row">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25" />
</svg>
      <nav class=" flex flex-row gap-5">
        <router-link to="/about">Login</router-link>
      </nav>
    </div>
  </div>
    <div class=" flex flex-row hover:bg-gradient-to-bl from-red-400 to-yellow-700 rounded-md bg-slate-200">
      <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
  <path stroke-linecap="round" stroke-linejoin="round" d="M2.25 12l8.954-8.955c.44-.439 1.152-.439 1.591 0L21.75 12M4.5 9.75v10.125c0 .621.504 1.125 1.125 1.125H9.75v-4.875c0-.621.504-1.125 1.125-1.125h2.25c.621 0 1.125.504 1.125 1.125V21h4.125c.621 0 1.125-.504 1.125-1.125V9.75M8.25 21h8.25"/>
</svg>
      <button>
        Logout
      </button>
    </div>
  </div>
</section>


<section>
  <main>
    <div class=" flex flex-row items-center justify-center
     bg-gradient-to-r from-gray-600 to-slate-800  gap-5 py-20">
        <!---flexbox--->
        
        <div>
            <img class=" pt-7 h-80 w-80 rounded-r-3xl rounded-t-3xl overflow-hidden" src="./assets/images/1.jpg" alt="">
            <div class="flex flex-col gap-3 text-center pt-3">
                <p>Welcome to <span class=" text-3xl font-serif font-bold text-white">Poppy Schools</span></p>
                <span class=" font-bold text-2xl">Unlock Your Possibilities</span>
            </div>
        </div>
        <!---Login space--->
        <div>
            <div class=" text-center font-bold pb-10">
                <h3 class=" text-3xl">
                    Login Buddy
                </h3>
            </div>
            <div class=" flex flex-col gap-2">
                <span class=" flex flex-col text-center gap-1">
                    Name:{{ Name }}
                    <input class=" rounded-md" type="text" v-model="Name">
                </span>
                <span class=" flex flex-col text-center gap-1">
                    email:{{ email }}
                    <input class=" rounded-md" type="text" v-model="email">
                </span>
                <span class=" flex flex-col text-center gap-1">
                    contact:{{ contact }}
                    <input class=" rounded-md" type="text" required v-model="contact">
                </span>
                <span class=" flex flex-col text-center gap-1">
                    password:{{ password }}
                    <input class=" rounded-md" type="text" required v-model="password">
                </span>
                <div>
                    <button class=" flex my-6 p-4 ml-36 hover:bg-blue-400
                     bg-red-400 rounded-md  text-white" @click="saveData(haveID)">Login</button>
                </div>
            </div>
        </div>
    
    </div>

    <section>
        <!---add student details--->
        <!---main div--->
        <div class=" bg-zinc-700">
            <!--h1 div--->
            <div>
                <h1 class=" font-serif pt-20 pb-20 text-4xl align-middle
                  text-center font-bold border border-rose-700">
                    Student details
                </h1>
            </div>
        </div>
        <!---table div--->
        <div class=" text-white flex flex-row items-center justify-center
         bg-gradient-to-r from-gray-600 to-slate-800 ">
            <table>
                <thead>
                    <tr class="bg-gradient-to-r from-gray-600 to-slate-800 text-white ">
                        <th scope="col" class=" py-8 px-8 text-2xl">Name</th>
                        <th  scope="col" class=" py-8 px-6 text-2xl">Email</th>
                        <th  scope="col" class=" py-8 px-6 text-2xl">Contact</th>
                        <th  scope="col" class=" py-8 px-6 text-2xl">Password</th>
                        <th  scope="col" class=" py-8 px-6 text-2xl">Action</th>
                    </tr>
                </thead>
                <tbody>
                    <tr class=" bg-gradient-to-r from-gray-600 to-slate-800  bg-white
                     border-b border-dashed" v-for="data in Poppy" :key="data.id">
                        <td class=" px-8 py-4">
                            {{ data.Name }}
                        </td>
                        <td class=" px-8 py-4">
                            {{ data.email }}
                        </td>
                        <td class=" px-8 py-4">
                            {{ data.contact }}
                        </td>
                        <td class=" px-8 py-4">
                            {{ data.password }}
                        </td>
                        <td class=" px-8 py-4">
                            <div>
                                <button class=" bg bg-blue-700 hover:bg-blue-400
                                 font-bold py-2 px-4 rounded-1" @click="deleteData(data.id)">
                                    Delete
                                </button>
                            </div>
                        </td>
                    </tr>
                </tbody>
            </table>
        </div>
    </section>
   </main>
</section>

</main>
  <router-view/>
</template>

<script>
    export default {
        data() {
            return {
                Name:'',
                email:'',
                contact:'',
                password:'',
                haveID:null,

                Poppy:[
                
                ]

            }
        },
        methods: {
            deleteData(id){
                //index is index of id we want to delete
                var index= this.Poppy.findIndex((data)=>data.id==id)
                console.log(index);

                this.Poppy.splice(index, 1)
            },
            getData(id){
                this.haveID=id
                var dataObj= this.Poppy.filter((data)=>(data.id==id))
                //assign to input 
               this.Name=dataObj[0].Name
               this.email=dataObj[0].email
               this.contact=dataObj[0].contact
               this.password=dataObj[0].password
            },
            saveData(haveID){
                //UPDATE DATA
                if (haveID) {
                    var dataObj= this.Poppy.filter((data)=>(data.id==id))
                    dataObj[0].Name=this.Name
                    dataObj[0].email=this.email
                    dataObj[0].contact=this.contact
                    dataObj[0].password=this.password
                }else{
                    //add data
                    const id=this.Poppy.length + 1
                    const data =
                    {
                        id:id,
                        Name:this.Name,
                        email:this.email,
                        contact:this.contact,
                        password:this.password
                    }
                    this.Poppy.push(data);
                }
            }   
        },
    }
</script>
<style>

</style>
