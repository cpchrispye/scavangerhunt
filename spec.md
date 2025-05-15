A signle html webpage that will be for mobile. it will be a used as a quiz form for a savanger hunt. the layout will be:
Title
Question
user input (either text box or multiple choice)
submit

the will be a json file call questions.json next to the html file in the format of

{
	q1:{
		title:"my title",
		question:"my question",
		type:"text",
		answer:"my answer"
		success_text: "congrats!",
		success_link: "link_to_google_maps",
	}
	q2:{
		title:"my title",
		question:"my question",
		type:"radio",
		answers:["answer_1", "answer_2", "answer_3", "answer_4"]
		answer:2
		success_text: "congrats!",
		success_link: "link_to_google_maps",
	}
}

if the submitted answer is wrong the submit button should go red until the answer is changed then it resets to the default colour. the button should disappear on success, and the input should be locked.
text answers should have the inpur stripped of preccedding and trailing whitespace, and all answers should be compared in lowercase.

the web page should know what quesion to display based on the argument provide in the url domain.com/my/page?q=q1
if no arg is given show the first question.

the success_link is optional, it could be a picture or a map link, it should be displayed after the success text. in a frame, clicking on it should open up the link. the link should make good use of teh space remaining.
 this will be hosted on github pages, so it must be static, ideally vanialla JS, css html, all inlined in the html.
