# Basic layer breakdown

This is a very minimal layer with minimal features. Most things will require additional features.

```js
addLayer("p", {
    startData() { return {                  
        unlocked: true,                     
        points: new Decimal(0),            

    color: "#4BDC13",                       
    resource: "prestige points",           
    row: 0,                                 

    baseResource: "points",                 
    baseAmount() { return player.points },  

    requires: new Decimal(10),              
                                            

    type: "normal",                        
    exponent: 0.5,                         

    gainMult() {                            
        return new Decimal(1)               
    },
    gainExp() {                             
        return new Decimal(1)
    },

    layerShown() { return true }           
})
```
