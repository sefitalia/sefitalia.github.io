// Place your application-specific JavaScript functions and classes here
// This file is automatically included by javascript_include_tag :defaults

jQuery(function($){//on document ready
  //autocomplete
  $('input.autocomplete').each(function(){
    var input = $(this);
    input.autocomplete(input.attr('autocomplete_url'),{
      matchContains:1,//also match inside of strings when caching
      //    mustMatch:1,//allow only values from the list
      //    selectFirst:1,//select the first item on tab/enter
      removeInitialValue:0//when first applying $.autocomplete
    });
  }); 

 $('a[rel*=facebox]').facebox();
});



function clickclear(thisfield, defaulttext) {
	if (thisfield.value == defaulttext) {
	thisfield.value = "";
	}
	}

function clickrecall(thisfield, defaulttext) {
	if (thisfield.value == "") {
	thisfield.value = defaulttext;
	}
}

function commaCheck(e){
	isIE=document.all? 1:0
	keyEntry = !isIE? e.which:event.keyCode; 
	if(keyEntry == '46')
		{return true; }
		
	if(keyEntry == '8')
		{return true; }
		
	if((keyEntry < '48') || (keyEntry > '57'))
				{return false;  }
				
	if(keyEntry == '44')
			{return false;  }
	

}

	
	
function alert4(id){
	Ext.Msg.show({
   		title:'Attenzione',
   		msg: 'Vuoi creare un listino dove inserire questo prodotto?',
   		buttons: Ext.Msg.YESNOCANCEL,
   		animEl: 'elId',
   		fn: destination4,
   icon: Ext.MessageBox.QUESTION
	});


function destination4(btn){
	if(btn == "yes"){
		window.open ("/admin/products/pb_new?passed_id="+id,"_self");
	}else if(btn == "no"){
		window.open ("/admin/questions/of_to_pricebook/"+id,"_self");
	}else if(btn == "cancel"){
	}
   };

}

function alert3(id){
	Ext.Msg.show({
   		title:'Attenzione',
   		msg: 'Vuoi creare una richiesta dove inserire questo prodotto?',
   		buttons: Ext.Msg.YESNOCANCEL,
   		animEl: 'elId',
   		fn: destination3,
   icon: Ext.MessageBox.QUESTION
	});


function destination3(btn){
	if(btn == "yes"){
		window.open ("/admin/products/pb_new?passed_id="+id,"_self");
	}else if(btn == "no"){
		window.open ("/admin/questions/req_to_pricebook/"+id,"_self");
	}else if(btn == "cancel"){
	}
   };

}

function alert5(id){
	Ext.Msg.show({
   		title:'Attenzione',
   		msg: 'Vuoi creare un listino dove inserire questo prodotto?',
   		buttons: Ext.Msg.YESNOCANCEL,
   		animEl: 'elId',
   		fn: destination5,
   icon: Ext.MessageBox.QUESTION
	});


function destination5(btn){
	if(btn == "yes"){
		window.open ("/admin/products/pb_new?passed_id="+id,"_self");
	}else if(btn == "no"){
		window.open ("/admin/questions/inq_to_pricebook/"+id,"_self");
	}else if(btn == "cancel"){
	}
   };

}

function show_product(id){
	window.open ("/store/show/"+id,"_self");
}

function show_product_ws(id){
	window.open ("/warehouses/show/"+id,"_self");
}

function partner(id){
	window.open ("/store/partner/"+id,"_self");
}

function show_user(id){
	window.open("/admin/users/custEdit/"+id,"_blank");
}

function showsTooltip(id){
	var my_tooltip = new Tooltip(id, 'tooltip_'+id)
}

function addUserSpot() {
	var new_upload_box = $('users_empty_country_upload').cloneNode(true);
	new_upload_box.style.display = "none";
	new_upload_box.id = '';
	$('users_country_container').appendChild(new_upload_box);
	new Effect.Appear(new_upload_box);
}


function addEmptyCountry() {
	var box = $('.upload_box').clone();
	box.removeClass("upload_box").fadeIn('slow').appendTo('.empty_upload');
}

function addEmptyProduct() {
	var box = $('.upload_product_box').clone();
	box.removeClass("upload_product_box").fadeIn('slow').appendTo('.product_upload');
}

function addEmptyProductBox() {
	var box = $('.upload_new_product_box').clone();
	box.removeClass("upload_new_product_box").fadeIn('slow').appendTo('.product_upload_box');
}

function addEmptyTiprod() {
	var box = $('.upload_box').clone();
	box.removeClass("upload_box").fadeIn('slow').appendTo('.empty_upload');
}

function addEmptyCategory() {
	var box = $('.category_box').clone();
	box.removeClass("category_box").fadeIn('slow').appendTo('.empty_category');
}

function addExcludedNation(a) {
	var box = $('.' + a + '_upload_box').clone();
	box.removeClass(a + '_upload_box').fadeIn('slow').appendTo('.' + a + '_empty_upload');
}

function addEmptyProductComplete() {
	var box = $('.upload_new_product_complete_box').clone();
	box.removeClass("upload_product_complete_box").fadeIn('slow').appendTo(".empty_upload");
}



function showWarehouse(id) {
     window.document.title = document.getElementById(id.toString()).value;
     getMyApp("tesXML").showWarehouse("1");
 }

 function getMyApp(appName) {
     if (navigator.appName.indexOf ("Microsoft") !=-1) {
         return window[appName];
     } else {
         return document[appName];
     }
 }

