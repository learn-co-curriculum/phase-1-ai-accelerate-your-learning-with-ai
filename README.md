# Accelerate Your Learning with AI

## Learning Goals

- Describe the known-unknown matrix.
- Discuss guidelines on using AI for learning.

## Introduction

In previous lessons, we discussed how AI chatbots are used by software engineers
and the limitations of such tools. In this lesson, we will look at the
known-unknown matrix and explore how we can leverage AI chatbots for learning
programming concepts.

## The Known-Unknown Matrix

The known-unknown matrix is a design thinking tool that helps to identify one’s
familiarity with a topic.

|         | Known                                                                | Unknown                                    |
| ------- | -------------------------------------------------------------------- | ------------------------------------------ |
| Known   | Information or knowledge we think are true.                          | Information gaps or risks we are aware of. |
| Unknown | Information we know are true based on experiences but can’t explain. | Information we are not aware of at all.    |

Let’s look at examples for each of the quadrants to better understand the
concept:

- **Known-knowns:** There are some fundamental programming principles you are
  aware of such as variable declarations and looping. You can use these ideas in
  your preferred programming language.
- **Known-unknowns:** Even if you exclusively use 1 or 2 programming languages,
  you may be aware of the existence of other programming languages. You know
  that they exist but aren’t aware of their data model or syntax.
- **Unknown-knowns:** You may use built-in or external functions and libraries
  in your application without fully understanding how they work. For example,
  you may use the `sort` method in JavaScript to sort an array without knowing
  what type of sorting algorithm is being used. You know from reading the docs
  and experience how to use the method but can’t explain how or why it works.
- **Unknown-unknowns:** These are things you don’t know exist. For example, if
  you have been only using programming languages that have loops, you may not be
  aware of languages that don’t have them (uses recursion instead).

How does labeling our knowledge help us effectively use AI chatbots? One of the
main issues with these chatbots is their propensity to respond with completely
false information with absolute certainty. If you’re unsure about your
familiarity with a topic, chatbots may guide you in the wrong direction.

Here’s an
[exchange between a JS developer with 20+ years of experience and ChatGPT](https://www.linkedin.com/posts/getify_where-do-i-send-my-invoice-for-teaching-activity-7005600563258146816-Vdg1/?utm_source=share&utm_medium=member_desktop).
In this case, Kyle asked a question that can be categorized as a known-known to
him. He immediately knew that ChatGPT’s answer was wrong.

But if someone who wasn’t aware of the `parseInt` method and JavaScript’s type
coercion rules asked this question, they may have taken ChatGPT’s answer for
granted and miss the nuances. However, if they are aware of their lack of
knowledge on the topic, they would seek out external sources for validation.

It’s important to know the limits of our knowledge so we know how to address
them. A software engineer may have to work with multiple unfamiliar languages
and tools at their job. This framework allows us to label our knowledge gaps,
frame them in the context of our experiences, and then address them depending on
the quadrant it’s in.

And finally, when you are learning something notice how your understanding of
the topic is evolving. If you start at a specific stage and aren’t making
progress, you should revise your learning strategy or seek out help.

Check out [this article](https://stephen.fm/known-unknown-matrix/) and
[this article](https://miro.com/miroverse/knownunknown-matrix-69w3bdmau9ayprzn/)
for more on this subject.

## Guidelines for Using AI Chatbots for Learning

In order to make the most of AI chatbots, we have to be aware of their
limitations and structure our prompts accordingly. Here are some general
guidelines that can help keep the chatbot from going off track:

1. **Start Simple:** You may encounter several complex prompts when researching
   online. But it’s completely fine to start with simple questions about
   concepts you want to learn more about and ask follow-up questions for further
   clarifications.
2. **Code Examples:** Chatbots can generate code samples along with line-by-line
   explanations for the code they generate. You can ask the chatbot to “provide
   examples to explain the concept of callbacks” as a starting point and then
   ask clarifications on specific parts of the code.
3. **Real-world Examples:** Chatbots can also provide case studies and show how
   concepts you may already know relate to new concepts you’re trying to learn.
   For example, when you’re learning about sorting, you can ask the chatbot,
   “what are some real-world applications of sorting algorithms?” and it will
   tell you about their role in search engines, databases, contact lists with
   detailed overview.
4. **Code Tracing:** Chatbots can provide a step-by-step walkthrough of code
   snippets along with explanations for each step. Provide the chatbot with your
   code snippet and ask it to “trace the execution path of the following code in
   <language name>”.
5. **Custom Quizzes:** Custom quizzes can be generated on specific topics. Ask
   the chatbot, “give me a 3 question quiz challenge on JavaScript closures”. If
   it shows the answers along with the questions, you may have to add “don’t
   show the answers until I’ve tried to solve the questions” to the prompt.
6. **Custom Code Challenges:** We can also ask the chatbot to ask us a code
   challenge with the prompt, “give me a code challenge on closure in
   JavaScript”.
7. **Validate with External Resources:** If you are learning something and
   you’re not fully sure about the topic, validate the information provided by
   the chatbot with external sources. Ideal sources are official documentations,
   books, and high quality articles.

## Custom Quiz Example

Here’s the user prompt:

```
Give me  a 3 question quiz challenge on JavaScript closures. Don't show the answers with the question.
```

And here’s the initial ChatGPT response with the questions:

```
Certainly! Here's a three-question quiz challenge on JavaScript closures. The answers will be provided separately after each question:

Question: What is the output of the following code snippet?

function outer() {
  var x = 10;
  function inner() {
    console.log(x);
  }
  return inner;
}

var closureFunc = outer();
closureFunc();

Question: Which of the following statements about closures in JavaScript is true?
	a) Closures are created when a function is defined.
	b) Closures only retain references to variables passed as arguments to inner functions.
	c) Closures cannot access variables from outer scopes.
	d) Closures are not used in modern JavaScript programming.

Question: In JavaScript, what happens if a closure references a variable that has been modified or reassigned after the closure was defined?
	a) The closure automatically updates to reflect the modified value.
	b) The closure retains the original value of the variable.
	c) The closure loses access to the variable and throws an error.
	d) The behavior depends on how the closure is invoked.
```

User prompt answering the questions:

```
Answer A: logs the value 10.
Answer B: A
Answer C: B
```

ChatGPT feedback response:

```
Great effort! Here are the correct answers:

Answer: The output of the code snippet will be 10.

Answer: The correct statement about closures in JavaScript is: a) Closures are created when a function is defined.

Answer: If a closure references a variable that has been modified or reassigned after the closure was defined, the closure retains the updated value. Therefore, your answer, option B, is correct.

Well done! If you have any more questions or need further clarification, feel free to ask!
```

Try asking it to create a code challenge in a similar manner. The challenges can
be pretty fun!

## Conclusion

AI chatbots are excellent tools for supporting education. General-purpose
chatbots aren’t specifically designed for helping learners but they still offer
powerful tools such as custom quiz generation and challenge generation, code
walkthroughs, and code explanations.

Experiment with different ways of using a chatbot for learning. Occasionally
reinforce your skills and knowledge through quizzes and challenges to ensure
you’re retaining information. Remember that the guidelines are for helping you
to get started but you can direct your own learning by leveraging these amazing
chatbots!
