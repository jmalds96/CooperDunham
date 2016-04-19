var main = function(){
    /*$('.dropdown-toggle').click(function(){
       $('.dropdown-menu').toggle(); 
    });*/
    
    $('.showmore').click(function(e){
    		$('.more').show(200);
    		$('.general').hide();
    		e.preventDefault();
    });
    
    $('.showless').click(function(e){
    		$('.more').hide(200);
    		$('.general').show();
    		e.preventDefault();
    });
    
    $('.arrow-next').click(function(e){
        var currentSlide = $('.active-slide');
        var nextSlide = currentSlide.next();
        if(nextSlide.length === 0){
            nextSlide=$('.slide').first();
        }
        currentSlide.fadeOut(500).removeClass('active-slide');
        nextSlide.fadeIn(500).addClass('active-slide');
        var currentDot = $('.active-dot');
        var nextDot = currentDot.next();
        if(nextDot.length === 0){
            nextDot=$('.dot').first();   
        }
        currentDot.removeClass('active-dot');
        nextDot.addClass('active-dot');
        e.preventDefault();
    });
    
    $('.arrow-prev').click(function(e){
        var currentSlide = $('.active-slide');
        var prevSlide = currentSlide.prev();
        if(prevSlide.length === 0){
            prevSlide=$('.slide').last();
        }
        currentSlide.fadeOut(500).removeClass('active-slide');
        prevSlide.fadeIn(500).addClass('active-slide');
        var currentDot = $('.active-dot');
        var prevDot = currentDot.prev();
        if(prevDot.length === 0){
            prevDot=$('.dot').last();   
        }
        currentDot.removeClass('active-dot');
        prevDot.addClass('active-dot');
        e.preventDefault();
    });
    
    setInterval(function(){
    	var currentSlide = $('.active-slide');
        var nextSlide = currentSlide.next();
        if(nextSlide.length === 0){
            nextSlide=$('.slide').first();
        }
        currentSlide.fadeOut(1000).removeClass('active-slide');
        nextSlide.fadeIn(1000).addClass('active-slide');
        var currentDot = $('.active-dot');
        var nextDot = currentDot.next();
        if(nextDot.length === 0){
            nextDot=$('.dot').first();   
        }
        currentDot.removeClass('active-dot');
        nextDot.addClass('active-dot');
    },10000);
    
    $('.dropdown-toggle').click(function() {
    		var location = $(this).attr('href');
    		window.location.href = location;
    		return false;
    });
}

$(document).ready(main);