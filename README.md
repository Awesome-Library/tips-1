tips
===
CSS tooltips with minimal effort!

![alt tag](https://raw.github.com/jh3y/screenshots/master/tips/tips.gif)

##example

    <a data-tip="true" data-tip-content="I'm a tooltip!" class="top"></a>

Tooltips shouldn't be complicated and they shouldn't do more than what's absolutely necessary. If your tooltips need to do more than just supply a small snippet of info then consider your design or consider using something like a popover component instead maybe.

##no js required
Tooltips should be simple and as such, so is this implementation.

By default `tips` will work on `hover` when viewing from a desktop environment.

On mobile devices, due to the nature of how `hover` behaves, tapping will work to show and hide `tips`.

If you do want to use javascript to trigger the showing and hiding of `tips` you can do simply by toggling the class `show` on the element that has a tip.

    var tip = document.getElementById('myTip');
    tip.className += ' show';

Or with jQuery maybe

    $('#myTip').toggleClass('show');


##how does this work?
`tips` is simply taking advantage of pseudo elements `:before` and `:after`.

##how do I change the colors? sizes? etc.
`tips` is available in both `less` and `sass` versions and has various variables for things like color and size that can be changed. There are two sizing helper classes included for `small` and `large` tips.

##contributing
As always any suggestions etc. are welcome!
Tweet me @ `_jh3y` or submit an issue!

__@jh3y__
