const CLIENT_ID = 'keECa1lpVtgABa1F';
const splash=document.querySelector('.splash');
const stuffjs=document.querySelector('.stuff');
const memberlist=document.querySelector('.members-list')
const messagelist=document.querySelector('.messages')
const msgforminput=document.querySelector('.message-form__input');
const msgformbutton=document.querySelector('.message-form__button');
const settingsbutton=document.querySelector('.settingsbutton');
const settings=document.querySelector('.settings');
const credit=document.querySelector('.credit')
var darkmode;
var isDarkMade;
var darkmodeselect;
/*const settingsimg=document.querySelector('.settingsimg');*/

const collapsesetting=document.querySelector('.collapsesettings');

var isSettingPressed=false;
function addButton(val,color,color2){
  darkmode=document.createElement("button",value=val )
  darkmode.classList.add('darkmode')
  settings.appendChild(darkmode)
  darkmode.innerHTML="Enable Dark Mode"
  darkmodeselect=document.querySelector('.darkmode');
  isDarkMade=true;
  darkmodeselect.addEventListener('click',(e)=>{
    console.log('this works')
    
    console.log('this still works')
    
    document.body.style.background = color;
    document.body.style.color= color2;
    msgforminput.style.background=color;
    msgforminput.style.color=color2;
    msgformbutton.style.background=color;
    msgformbutton.style.color=color2;
    collapsesetting.style.background=color;
    collapsesetting.style.color=color2;
    settingsbutton.style.color=color2;
    settingsbutton.style.background=color;
  })
}
var usermade;
var drone;

/*function createMenuItem(name) {
  let inputname = document.createElement('input');
  inputname.placeholder = name;
  inputname.className='inputnamefield';
  return inputname;
}*/
/*function createButton(btnname){
  let btn = document.createElement('input');
  btn.type = 'submit';
  btn.className='submitbtn';
  return btn;
}*/

const inputnamefield = document.querySelector('.inputnamefield');
const button = document.querySelector('.submitbtn');
  // multi tab detection
  function register_tab_GUID() {
    // detect local storage available
    if (typeof (Storage) !== "undefined") {
        // get (set if not) tab GUID and store in tab session
        if (sessionStorage["tabGUID"] == null) sessionStorage["tabGUID"] = tab_GUID();
        var guid = sessionStorage["tabGUID"];

        // add eventlistener to local storage
        window.addEventListener("storage", storage_Handler, false);

        // set tab GUID in local storage
        localStorage["tabGUID"] = guid;
    }
}

function storage_Handler(e) {
    // if tabGUID does not match then more than one tab and GUID
    if (e.key == 'tabGUID') {
        if (e.oldValue != e.newValue) tab_Warning();
    }
}

function tab_GUID() {
    function s4() {
        return Math.floor((1 + Math.random()) * 0x10000)
          .toString(16)
          .substring(1);
    }
    return s4() + s4() + '-' + s4() + '-' + s4() + '-' +
      s4() + '-' + s4() + s4() + s4();
}

function tab_Warning() {
    alert("Another tab is open! Please close this tab so you can return to your work. We do not allow users to have multiple tabs open because the API we are using has a limit of 20 concurrent users. ");
    if(usermade!==true){
    button.parentElement.removeChild(button)
    inputnamefield.parentElement.removeChild(inputnamefield)
    }

    msgformbutton.parentElement.removeChild(msgformbutton)
    msgforminput.parentElement.removeChild(msgforminput)
    messagelist.parentElement.removeChild(messagelist)
    memberlist.parentElement.removeChild(memberlist)
    if(usermade==true){
    drone.close();
  
    }
}

settingsbutton.addEventListener('click',(e)=>{
  isSettingPressed=true;
  addButton("Dark Mode",'black','white')
  settingsbutton.classList.add('disable')
  /*settingsimg.classList.add('disable')*/
  document.querySelector('.settingsbutton').disabled = 'true';
  /*document.querySelector('.settingsimg').disabled = 'true';*/
})
collapsesetting.addEventListener('click',(e)=>{
  darkmode.parentNode.removeChild(darkmode)
  document.querySelector('.settingsbutton').disabled = false;
  /*document.querySelector('.settingsimg').disabled = false;*/
})

button.addEventListener('click', (e) => {
   setTimeout(() => {
       const yourname = inputnamefield.value
       button.classList.add('display-none');
       
       usermade=true;
       inputnamefield.parentElement.removeChild(inputnamefield);
       button.parentElement.removeChild(button);
       drone = new ScaleDrone(CLIENT_ID, {
        data: { // Will be sent out as clientData via events
          name: yourname,
          color: getRandomColor(),
        },
      });
      let members = [];

      drone.on('open', error => {
        if (error) {
          return console.error(error);
        }
        console.log('Successfully connected to Scaledrone');
      
        const room = drone.subscribe('observable-room');
        room.on('open', error => {
          if (error) {
            return console.error(error);
          }
          console.log('Successfully joined room');
        });
      
        room.on('members', m => {
          members = m;
          updateMembersDOM();
        });
      
        room.on('member_join', member => {
          members.push(member);
          updateMembersDOM();
        });
      
        room.on('member_leave', ({id}) => {
          const index = members.findIndex(member => member.id === id);
          members.splice(index, 1);
          updateMembersDOM();
        });
      
        room.on('data', (text, member) => {
          if (member) {
            addMessageToListDOM(text, member);
          } else {
            // Message is from server
          }
        });
      });
      
      drone.on('close', event => {
        console.log('Connection was closed', event);
      });
      
      drone.on('error', error => {
        console.error(error);
      });
      
      function getRandomName() {
        const adjs = ["autumn", "hidden", "bitter", "misty", "silent", "empty", "dry", "dark", "summer", "icy", "delicate", "quiet", "white", "cool", "spring", "winter", "patient", "twilight", "dawn", "crimson", "wispy", "weathered", "blue", "billowing", "broken", "cold", "damp", "falling", "frosty", "green", "long", "late", "lingering", "bold", "little", "morning", "muddy", "old", "red", "rough", "still", "small", "sparkling", "throbbing", "shy", "wandering", "withered", "wild", "black", "young", "holy", "solitary", "fragrant", "aged", "snowy", "proud", "floral", "restless", "divine", "polished", "ancient", "purple", "lively", "nameless"];
        const nouns = ["waterfall", "river", "breeze", "moon", "rain", "wind", "sea", "morning", "snow", "lake", "sunset", "pine", "shadow", "leaf", "dawn", "glitter", "forest", "hill", "cloud", "meadow", "sun", "glade", "bird", "brook", "butterfly", "bush", "dew", "dust", "field", "fire", "flower", "firefly", "feather", "grass", "haze", "mountain", "night", "pond", "darkness", "snowflake", "silence", "sound", "sky", "shape", "surf", "thunder", "violet", "water", "wildflower", "wave", "water", "resonance", "sun", "wood", "dream", "cherry", "tree", "fog", "frost", "voice", "paper", "frog", "smoke", "star"];
        return (
          adjs[Math.floor(Math.random() * adjs.length)] +
          "_" +
          nouns[Math.floor(Math.random() * nouns.length)]
        );
      }
      
      function getRandomColor() {
        return '#' + Math.floor(Math.random() * 0xFFFFFF).toString(16);
      }
      
      //------------- DOM STUFF
      
      const DOM = {
        membersCount: document.querySelector('.members-count'),
        membersList: document.querySelector('.members-list'),
        messages: document.querySelector('.messages'),
        input: document.querySelector('.message-form__input'),
        form: document.querySelector('.message-form'),
      };
      
      DOM.form.addEventListener('submit', sendMessage);
      
      function sendMessage() {
        const value = DOM.input.value;
        if (value === '') {
          return;
        }
        DOM.input.value = '';
        drone.publish({
          room: 'observable-room',
          message: value,
        });
      }
      
      function createMemberElement(member) {
        const { name, color } = member.clientData;
        const el = document.createElement('div');
        el.appendChild(document.createTextNode(name));
        el.className = 'member';
        el.style.color = color;
        return el;
      }
      
      function updateMembersDOM() {
        DOM.membersCount.innerText = `${members.length} users in room:`;
        DOM.membersList.innerHTML = '';
        members.forEach(member =>
          DOM.membersList.appendChild(createMemberElement(member))
        );
      }
      
      function createMessageElement(text, member) {
        const el = document.createElement('div');
        el.appendChild(createMemberElement(member));
        el.appendChild(document.createTextNode(text));
        el.className = 'message';
        return el;
      }
      
      function addMessageToListDOM(text, member) {
        const el = DOM.messages;
        const wasTop = el.scrollTop === el.scrollHeight - el.clientHeight;
        el.appendChild(createMessageElement(text, member));
        if (wasTop) {
          el.scrollTop = el.scrollHeight - el.clientHeight;
        }
      }










   }, 1);
})





document.addEventListener('DOMContentLoaded',(e)=>{
  setTimeout(()=>{
    splash.classList.add('display-none');
    splash.parentElement.removeChild(splash);
    register_tab_GUID()
    console.log(msgformbutton)
  },2000);
})
splash.addEventListener('mousedown',
(e)=>{
  setTimeout(()=>{
    splash.parentElement.removeChild(splash);
    
  },1);
})
 



