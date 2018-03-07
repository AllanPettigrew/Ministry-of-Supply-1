A Pen created at CodePen.io. You can find this one at https://codepen.io/AllanPettigrew/pen/oEOgRJ.



// Down Arrow "Bounce Scroll Down Arrow A PEN BY Yannick Bisaillon"

.fa-chevron-down {
  display: block;
  margin: 0 auto;
  margin-bottom: 90px;
  animation: 
    bounce 
    5s
    infinite;
}

@keyframes bounce {
  0%, 20%, 50%, 80%, 100% {
    transform: translateY(0);
  }
  30% {
    transform: translateY(-15px);
  }
  60% {
    transform: translateY(-15px);
  }
  90% {
    transform: translateY(-15px);
  } 
} 


// Author Cory LaViska / Smooth scroll

$('a[href^="#"]').on('click', function(event) {

    var target = $(this.getAttribute('href'));

    if( target.length ) {
        event.preventDefault();
        $('html, body').stop().animate({
            scrollTop: target.offset().top
        }, 1000);
    }

});

