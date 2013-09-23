/* 
 * To change this template, choose Tools | Templates
 * and open the template in the editor.
 */

$(function(){
    
    $("#next").bind("click",function(){
       enableButtons(buttonsArr,false)
        TweenLite.to($('#frame'),.8,{rotationX:"+=90",ease:Back.easeOut,onComplete:enableButtons,onCompleteParams:[buttonsArr]});
    });
     $("#prev").bind("click",function(){
       enableButtons(buttonsArr,false)
       TweenLite.to($('#frame'),.8,{rotationX:"-=90",ease:Back.easeOut,onComplete:enableButtons,onCompleteParams:[buttonsArr]});
    });

});
var buttonsArr=['#prev','#next'];
var enableButtons=function(btnsArr,flag){ 
    for(var b=0; b<btnsArr.length; b++){
        if(flag===false){           
            $(btnsArr[b]).attr('disabled',true);
        }else{
            $(btnsArr[b]).removeAttr('disabled');
        }
    }
};

