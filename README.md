# Blueprint
1. [cart] checkbox -> useForm(react-hook-form) -> watch / may use [1] react-query to handle local state. [test first!]
- https://jacegem.github.io/blog/2018/localStorage-%EC%97%90-checkbox-%EC%83%81%ED%83%9C-%EC%A0%80%EC%9E%A5/
- https://stackoverflow.com/questions/26628812/localstorage-how-to-save-a-checkbox

2. checkout -> transaction [medium priority] - may use: [1] react-query to handle api state
strongly recommended to test out this feature first (before making the whole contents)
- https://velog.io/@sayi/React-%EC%B9%B4%EC%B9%B4%EC%98%A4-%ED%8E%98%EC%9D%B4%EA%B2%B0%EC%A0%9C-%EC%A4%80%EB%B9%84
- https://velog.io/@sayi/React-%EC%B9%B4%EC%B9%B4%EC%98%A4-%ED%8E%98%EC%9D%B4%EA%B2%B0%EC%A0%9C-%EC%8A%B9%EC%9D%B8

3. pages [high priority]
- CartPage: box container, inner box, 3-4 items to display it. scrollable depending on the list of added item.
- CheckOutPage: kakaopay module will be added/addressed here.
- Home: make first screen only. Don't scroll down.
- ProductDetailPage : same as 4, 5

4. product-details [low priority]
- just as simple as coupang.

5. product-list [high priority]
- just as simple as coupang.

6. utils
- this can be tricky. Consider making this part at the end once draft is complete. Refactoring purpose only.

# Plan
<!-- Do not apply CSS till whole major features are completed. -->
- page -> home : with no css, just set up basic menu and navbar or anything necessary.
- page -> productDetailpage : (same)
- page -> list page : (same)
- page -> cart : see #1 description

# intermediate plan
- And test out kakaopay module. First, make up the module api from checkout.js, then address it to paymentForm.js.
- react hook form, apply checkbox, and possibly try adding isDirty if possible, maybe use this to say insufficient deposit etc? (If that so, just apply default deposit to user (don't add login feature though. No DB will be added).)
- among this process, use react-query's state management to handling axios.
- [add change of checkbox to localstorage vs react hook form.]

If this project is over too early, consider adding some dummyjson as item list, and add pagination feature.

Deadline: 7th Apr Friday. 18:00PM (KR time)