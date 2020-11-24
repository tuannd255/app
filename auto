var solve = require('https://raw.githubusercontent.com/AZcaptcha/azcaptcha.js/master/index.js');
console.log(solve)
$(document).ready(function () {
    var resetHref = 'http://hn.gamethuvn.net/#auth/Reset.asp';
    var loginHref = 'http://hn.gamethuvn.net/#auth/login.asp?next=auth%2Fchecklogin1';
    var defaultHref = 'http://hn.gamethuvn.net/';
    var href = window.location.href;
    if (href !== defaultHref && href !== loginHref) {
      setInterval(() => {
        history.go(0);
        console.log('reset')
      }, 60000)
        if (href !== resetHref) {
            // window.location.href = resetHref;
        } else {
          setTimeout(() => {
            window.scrollTo(0, 300)
          }, 1000);
          $('input[type="checkbox"]').attr('name', 'ResetOnline');
          $('input[type="checkbox"]').attr('value', 1);
          $('input[type="checkbox"]').removeAttr('disabled');
          $('input[type="checkbox"]').get(0).click();
          $('input[name="captcha"]').get(0).focus();
          
          // if (($('input[name="captcha"]').length > 0)) {
          //   $('input[name="captcha"]').get(0).value = 645;
          //   $('button[type="submit"]').get(0).click();
          //   // for (var i = 0; i < ('.bootstrap-dialog-footer-buttons button').length; i++) {
          //   //   $('.bootstrap-dialog-footer-buttons button').get(i).click();
          //   // }
          // }
        }
    }
})
