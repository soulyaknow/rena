<template>
    <div class="min-h-screen w-screen flex flex-col bg-gray-200">
        <nav class="bg-gradient-to-r from-white via-white to-gray-300 sticky top-0 z-50">
            <div class="max-w-screen flex flex-wrap items-center justify-between mx-auto p-4">
                <div class="flex items-center space-x-3 rtl:space-x-reverse md:ml-20">
                    <div class="text-[30px] text-gray-400">Renalyn</div>
                </div>
                <div class="flex md:order-2 space-x-3 md:space-x-0 rtl:space-x-reverse">
                    <button type="button" class="text-slate-950 bg-white hover:bg-gray-400 hover:text-white focus:ring-4 focus:outline-none focus:ring-gray-300 font-medium rounded-lg text-sm px-4 py-2 text-center dark:bg-gray-600 dark:hover:bg-gray-700 dark:focus:ring-gray-800">Get Started</button>
                    <button @click="navStore.showNavar"
                    data-collapse-toggle="navbar-sticky" type="button" class="inline-flex items-center p-2 w-10 h-10 justify-center text-sm text-gray-500 rounded-lg md:hidden hover:bg-gray-100 focus:outline-none focus:ring-2 focus:ring-gray-200 dark:text-gray-400 dark:hover:bg-gray-700 dark:focus:ring-gray-600" aria-controls="navbar-sticky" aria-expanded="false">
                        <span class="sr-only">Open main menu</span>
                        <svg class="w-5 h-5" aria-hidden="true" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 17 14">
                            <path stroke="currentColor" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M1 1h15M1 7h15M1 13h15"/>
                        </svg>
                    </button>
                </div>
                <div :class="{ visible: navStore.navarState }"
                class="items-center justify-between hidden w-full md:flex md:w-auto md:order-1" id="navbar-sticky">
                    <ul class="flex flex-col p-4 md:p-0 mt-4 font-medium md:space-x-8 rtl:space-x-reverse md:flex-row md:mt-0">
                        <li>
                            <a href="#home" class="block py-2 px-3 text-slate-900 md:bg-transparent md:text-gray-600 md:p-0">Home</a>
                        </li>
                        <li>
                            <a href="#about" class="block py-2 px-3 text-slate-900 md:bg-transparent md:text-gray-600 md:p-0">About</a>
                        </li>
                        <li>
                            <a href="#portfolio" class="block py-2 px-3 text-slate-900 md:bg-transparent md:text-gray-600 md:p-0">Services</a>
                        </li>
                    </ul>
                </div>
            </div>
        </nav>
        <div class="flex-grow max-w-screen max-h-full flex flex-col items-center justify-between">
            <div class="md:grid lg:grid-cols-2 sm:grid-cols-1 grid-cols-1 w-full h-full" id="home">
                <div class="bg-transparent h-full text-gray-600 md:pb-[30px] border-2 bg-gray-200 md:block hidden">
                    <div class="flex flex-col md:mt-10 md:pt-10 md:ml-32 ml-4">
                        <h1 class="text-left font-bold md:text-[40px] text-[35px] font-sans">I AM A CREATIVE</h1>
                        <h1 class="text-left font-bold md:text-[80px] text-[40px]">WEB DESIGNER</h1>
                        <p class="pb-2 text-[20px]">
                            Hi Students! As a fellow student in programming, I undestand the importance of creating user-friendly 
                            interfaces for startups.
                        </p>
                        <div class="flex pt-10 md:mx-0 mx-auto">
                            <button class="bg-gray-300 text-slate-950 font-medium text-sm px-5 py-2.5 text-center me-4 mb-2 w-32 rounded hover:bg-gray-400 hover:text-white">Get Started</button>
                            <button class="bg-white  text-slate-950 font-medium text-sm px-5 py-2.5 text-center me-2 mb-2 w-32 rounded hover:bg-gray-400 hover:text-white">Portfolio</button>
                        </div>
                    </div>
                </div> 
                <div class="transparent h-full overflow-hidden bg-gray-200 md:block hidden">
                    <div class="md:ml-60">
                        <img src="../assets/rena.png"  class="h-full w-96">                        
                    </div>
                </div>
                <div class="bg-slate-600 h-full md:hidden block">
                    <div class="h-full w-full m-auto bg-gray-200 relative flex items-center justify-center">
                        <div class="relative">
                            <img src="../assets/rena.png" alt="image" class="mx-auto h-full w-96 z-50 opacity-80">                        
                        </div>  
                        <div class="absolute bottom-0 transform -translate-y-1/2 text-gray-600 bg-gray-200 w-full">
                            <div class="flex flex-col ml-4">
                                <h1 class="text-left font-bold text-[25px] font-sans">I AM A CREATIVE</h1>
                                <h1 class="text-left font-bold text-[35px]">WEB DESIGNER</h1>
                                <p class="pb-2 text-[12px]">
                                    Hi Students! As a fellow student in programming, I understand the importance of creating user-friendly 
                                    interfaces for startups.
                                </p>
                            </div>
                        </div>
                        <div class="absolute bottom-0 bg-transparent">
                            <div class="flex flex-col ml-4">
                                <div class="flex mx-auto pt-4">
                                    <button class="bg-gray-300 text-slate-950 font-medium text-sm px-5 py-2.5 text-center me-4 mb-2 w-32 rounded hover:bg-gray-400 hover:text-white">Get Started</button>
                                    <button class="bg-white text-slate-950 font-medium text-sm px-5 py-2.5 text-center me-2 mb-2 w-32 rounded hover:bg-gray-400 hover:text-white">Portfolio</button>
                                </div>
                            </div>
                        </div>                                             
                    </div>
                </div>
            </div>                     
            <div class="grid lg:grid-cols-2 sm:grid-cols-1 grid-cols-2 w-full h-full mt-10" id="about">
                <div class="transparent h-full bg-gray-200 ">
                    <div class="md:ml-32">
                        <img src="../assets/ren.png"  class="h-full w-96">                        
                    </div>
                </div>
                <div class="flex flex-col bg-transparent h-full md:pb-[30px] bg-gray-200">
                    <div class="grid grid-cols-1 w-full h-full">
                        <div class="md:flex grid md:grid-cols-3 grid-cols-1 md:h-16">
                            <button class="bg-gray-300 h-10 text-slate-950 font-medium text-sm px-5 py-2.5 text-center me-4 mb-2 md:w-32 w-full rounded hover:bg-gray-400 hover:text-white">About</button>
                            <button class="bg-white h-10 text-slate-950 font-medium text-sm px-5 py-2.5 text-center me-2 mb-2 md:w-32 w-full rounded hover:bg-gray-400 hover:text-white">Education</button>
                            <button class="bg-white  h-10 text-slate-950 font-medium text-sm px-5 py-2.5 text-center me-2 mb-2 md:w-32 w-full rounded hover:bg-gray-400 hover:text-white">Experience</button>
                        </div>
                        <div>
                            <span class="text-slate-950 text-[25px]">About me</span>
                            <h1 class="text-gray-600 md:text-[40px] text-[30px] font-bold">Know about more</h1>
                            <p class="pb-2 text-[15px] font-semibold text-gray-600">
                                "Hello, I'm Renalyn, an aspiring student in technology. Passionate about the ever-evolving world of technology, 
                                I am on a journey of exploration and learning. Eager to delve into the exciting realms of programming and innovation, 
                                I am dedicated to honing my skills and making meaningful contributions to the field. 
                                Join me on this tech-driven adventure!"
                            </p>
                        </div>
                    </div>
                </div>      
            </div>
            <div class="grid lg:grid-cols-2 md:grid-cols-2 grid-cols-1 w-full h-full mt-10" id="portfolio">
                <div class="transparent bg-gray-200">
                    <div class="md:ml-32">
                        <div class="md:w-[500px] h-full w-[80%] mx-auto">
                            <h1 class="text-center text-[25px] pb-4">Todo App</h1> 
                            <div class="flex items-center space-x-2 mb-4">
                                <input type="text" class="border p-2 rounded-md w-full" v-model="task" placeholder="Add a new task" />                               
                                <button class="bg-gray-300 text-slate-950 text-sm px-4 font-medium rounded-md text-[25px] h-10 hover:bg-gray-400 hover:text-white" @click="addTask">Add</button>
                            </div>
                            <input type="text" class="border border-gray-300 p-2 rounded-md w-full mb-4" placeholder="Search tasks" v-model="searchQuery"/>
                            <div class="flex flex-col mb-4">
                                <div class="flex mb-2 items-center header w-full h-10 bg-gradient-to-r from-gray-500 via-gray-400 to-gray-300 text-slate-800 text-center">
                                    <p class="flex-1 py-6">Details</p>
                                    <p class="flex-1 py-6">Action</p>
                                </div>
                                <div class="flex items-center header h-full w-full transparent text-gray-400 text-center" v-for="todo in filteredTodos" :key="todo.id">
                                    <div class="datas flex w-full h-full py-2 bg-gray-100 text-white mb-2">
                                        <p class="flex-1 text-xl text-slate-600" :class="{ check: todo.status }">{{ capitalizeFirstLetter(todo.details) }}</p>
                                        <p class="flex-1">
                                            <a href="#" class="mx-2 h-full border rounded text-xl shadow-md text-gray-600" @click="updateData(todo.id, todo.status)">
                                                {{ isClick ? 'Uncheck' : 'Check' }}
                                            </a>
                                            <a href="#" @click="removeTask(todo.id)" class="border rounded text-xl shadow-md text-gray-600">
                                                Remove
                                            </a>
                                        </p>
                                    </div>
                                </div>
                            </div>
                        </div>
                        <div class="flex mt-4 text-center transparent mr-auto">
                            <button class="items-center header md:w-[500px] w-[50%] mx-auto h-10  bg-gray-300 rounded hover:bg-gray-400 hover:text-white
                            text-slate-950 text-center" 
                                v-if="hasTasks" @click="clearAllTasks">
                                Clear All
                            </button>
                        </div>                   
                        <p class="text-center text-[15px] pt-4 w-80 mx-auto">
                            Daily plan, track and finish your to-do task lists whether they be simple grocery shopping lists,
                            daily habits tied to goals, single work tasks or complex multi-person projects.
                        </p>                   
                    </div>
                </div>
                <div class="transparent h-full bg-gray-200 md:mt-0 mt-4">
                    <div class="md:ml-32">
                        <div class="md:w-[500px] h-full w-[80%] mx-auto">
                            <h1 class="text-center text-[25px] pb-4">Jack `N Poy App</h1>
                            <div class="flex w-full h-full md:pl-20 pl-4">
                                <label class="py-2">Total Rounds: </label>
                                <input type="number" v-model="totalRounds" class="border p-2 rounded-md text-center"/>
                            </div>
                            <div class="flex flex-col mt-4">
                                <div class="grid grid-cols-2 text-xl">
                                    <div class="text-center w-full  text-slate-500">
                                        <h1 class="border-b-2 border-black">Human</h1>
                                        <p class="bg-green-200">{{ humanChoice }}</p>
                                    </div>
                                    <div class="text-center w-full  text-slate-500">
                                        <h1 class="border-b-2 border-black">Computer</h1>
                                        <p class="bg-red-200">{{ computerChoice }}</p>
                                    </div>
                                </div>
                                <div class="text-center text-xl bg-blue-400 mt-4">
                                    <p>{{ result }}</p>
                                </div> 
                                <div class="grid grid-cols-2 text-xl">
                                    <div class="text-center w-full  text-slate-500">
                                        <p>{{ humanWins }}</p>
                                    </div>
                                    <div class="text-center w-full  text-slate-500">
                                        <p>{{ computerWins }}</p>
                                    </div>
                                </div>                                                                                   
                            </div>
                            <div class="flex flex-col-3 mt-4 space-x-4 pb-10">
                                <button @click="play('rock')" class="w-full bg-green-400 rounded">Rock</button>
                                <button @click="play('paper')" class="w-full bg-red-400 rounded">Paper</button>
                                <button @click="play('scissors')" class="w-full bg-blue-400 rounded">Scissors</button>
                            </div>   
                            <p class="text-center text-[15px] pt-4 w-80 mx-auto">
                                A Rock, Paper, Scissors app is a simple game application where two players make simultaneous choices 
                                among three options: rock, paper, or scissors.<br> The game has the following rules:<br>
                            </p>   
                            <p class="flex w-48 mx-auto">
                                1.Rock crushes scissors.
                                2.Scissors cut paper.
                                3.Paper covers rock.
                            </p>                    
                        </div>          
                    </div>
                </div>     
            </div>
        </div>
        <footer class="transparent  dark:bg-gray-800 mt-20 bg-gradient-to-r from-white via-white to-gray-300">
            <div class="max-w-screen-xl flex flex-wrap items-center justify-between mx-auto p-4">
                <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400">
                    Renlayn Dulmiguez
                </span>
                <span class="flex flex-wrap items-center  text-sm font-medium text-gray-500 dark:text-gray-400 sm:mt-0">
                    @2023-2024
                </span>
            </div>
        </footer>
    </div>
</template>
<script setup>
import { useNavarStore } from '../stores/';
import { db } from '../firebase';
import { ref, onMounted, computed } from 'vue';
import { collection, addDoc, serverTimestamp, onSnapshot, orderBy, query, doc, deleteDoc, updateDoc, getDocs } from 'firebase/firestore';

const navStore = useNavarStore();
const task = ref('');
const todos = ref([]);
const searchQuery = ref('');
const status = ref(false);
const isClick = ref(false);
const choices = ['rock', 'paper', 'scissors'];
const humanChoice = ref(null);
const computerChoice = ref(null);
const result = ref('');
const humanWins = ref(0);
const computerWins = ref(0);
const totalRounds = ref(0);

const capitalizeFirstLetter = (str) => {
    return str.charAt(0).toUpperCase() + str.slice(1);
};

const addTask = async (e) => {
      e.preventDefault();
      try {
        await addDoc(collection(db, 'todo'), {
          details: task.value,
          status: status.value,
          date_created: serverTimestamp(),
        });
        task.value = '';
      } catch (e) {
        console.error('Error adding document: ', e);
      }
};

const getData = () => {
      const fsquery = query(collection(db, "todo"), orderBy('date_created','asc'));
      onSnapshot(fsquery,(querySnapshot) => {
        const newTasks = [];
        querySnapshot.forEach((doc) => {
          const datas = {
              id:doc.id,
              details:doc.data().details,
              status:doc.data().status,
            }
            newTasks.unshift(datas);
        });
        todos.value=newTasks;
      })
};

const updateData = (id, currentStatus) => {
      const fsquery = doc(db, 'todo', id);
      const newData = {
        status: !currentStatus,
      }
      isClick.value = !isClick.value;
      updateDoc(fsquery, newData)
      .then(() => {
        console.log('Document successfully updated.');
      })
      .catch((error) => {
        console.error('Error updating document:', error);
      });
};

const removeTask = async (id) => {
      try{
        await deleteDoc(doc(db,'todo',id))
      }catch(e){
        console.log(e);
      }
};

const hasTasks = computed(()=> {
      return todos.value.length > 0;
});

const clearAllTasks = async () => {
      try {
        const querySnapshot = await getDocs(collection(db, 'todo'));
        querySnapshot.forEach(async (doc) => {
          await deleteDoc(doc.ref);
        });
        todos.value = [];
      } catch (e) {
        console.log(e);
      }
};
const filteredTodos = computed(()=> {
      return todos.value.filter(todo => {
        return todo.details.toLowerCase().includes(searchQuery.value.toLowerCase());
      });
});

const play = (human) => {
  if (humanWins.value < totalRounds.value && computerWins.value < totalRounds.value) {
    humanChoice.value = human;
    computerChoice.value = getComputerChoice();
    result.value = determineWinner(human, computerChoice.value);
    updateScores(result.value);
  } else {
    alert('Game over! Reset to play again.');
  }
};

const getComputerChoice = () => {
  // Simple strategy: Exploit the human tendency to repeat the same move
  const lastHumanChoice = humanChoice.value;
  const possibleChoices = choices.filter(choice => choice !== lastHumanChoice);
  return possibleChoices[Math.floor(Math.random() * possibleChoices.length)];
};

const determineWinner = (human, computer) => {
  if (human === computer) {
    return 'It\'s a tie!';
  } else if (
    (human === 'rock' && computer === 'scissors') ||
    (human === 'paper' && computer === 'rock') ||
    (human === 'scissors' && computer === 'paper')
  ) {
    return 'You win!';
  } else {
    return 'Computer wins!';
  }
};

const updateScores = (result) => {
  if (result.includes('You win')) {
    humanWins.value++;
  } else if (result.includes('Computer wins')) {
    computerWins.value++;
  }
};

onMounted(()=> {
    getData()
})
</script>
<style scoped>
.visible {
  display: block !important;
}
.overflow-y-scroll::-webkit-scrollbar {
    display: none;
    width: 0px;
}
.overflow-y-scroll:hover::-webkit-scrollbar {
    display: block;
}
.overflow-y-scroll::-webkit-scrollbar-track {
    background-color: transparent;
}
.overflow-y-scroll::-webkit-scrollbar-thumb {
    background-color: rgb(8, 47, 73, 1);
    border-radius: 8px;
    width: 4px;
} 
.check {
    text-decoration: line-through;
    color: red;
}
</style>