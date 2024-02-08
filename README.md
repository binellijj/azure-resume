# Azure Hosted Resume
My own Azure hosted resume following [ACG project video](https://www.youtube.com/watch?v=ieYrBWmkfno&t=4285s). 

## First Steps

- Clone Github repo 
- Created main.js vistor counter code

```js
window.addEventListener('DOMContentLoaded', (event) =>{
    getVisitCount();
})

const functionApi = '';

const getVisitCount = () => {
    let count = 30;
    fetch(functionApi).then(response => {
        return response.json()
    }).then(response.json()
        console.log("Website called function API.");
        count = response.count;
        document.getElementById("counter").innerText = count;
    }).catch(function(error){
        console.log(error);
    });
    return count;
}
```
- Created CosmosDB
- Created Azure Function App
- Created bindings to CosmosDB and added host URL to Json file for testing

