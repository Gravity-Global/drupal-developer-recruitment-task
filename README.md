# Drupal developer recruitment task
Hello 👋🏼 braveheart. We are truely delighted to introduce you to a Drupal developer recruitment task. It was designed to provide more information about your experience with Drupal as well as architectural skills for our HR team involved in the recruitment process. You will be presented real life problem you might come across in future and we expect you to prepare a document with a plan of how to resolve it.

Please note, no actual coding is required, however make sure you are very specific about technical issues and explain details as you would explain it to another developer. As we are more than sure the problem can be approached in different ways, please explain why do you think your solution is the best and what were the other ones you rejected.

We really hope to see you shortly on board, good luck! 🤘🏼

## Problem
Dripfeed works with different financial institutions, therefore some of mechanisms applied to our websites are crafted specificaly for this industry. For instance, directive 2014/65/EU of the European Parliament forced investment related firms to apply additional layer of visitor segmentation. In general, website visitors should be asked whether they are private or institutional investors with proper training and knowledge. Based on a selection, some pages will be absolutely different, adjusted as per legal requirements to their target audience.

From a point of view of a website architect, pages are divieded into 3 sections:
* Pages exactly the same for private and institutional investors (like contact page, or about us),
* Pages similar for private and insitutional investors (some paragraphs or images are different),
* Pages not related in any way (pages that are displayed for specific investors only).

As the solution is required by law and it should leave no margin for a human error, we decided to get rid of a second case – it would be too easy to reveal content that is not meant for specific audience. Dripfeed simply uses pages that are shared for all investors or pages that are meant for specific investor even if the difference between investors is a matter of a few words. Please note editing a page for specific investor should NOT update corresponding page for another investor. Another very important fact to note is a CDN. Content structure for each of investors should be given unique URI space to avoid content caching for wrong investors.

Your task is to find out best approach to implement investor selector to a website and organize content as explained above. Steps below might be helpful in strating point:
1. Think about how to implement “Investor modal”, which allows you to select whether you are Private or Insitutional investor and how to store the selection (User doesn’t have to be logged in). note: this is a legal requirement to display this modal.
2. Think what happens after investor type selection. note: most of financial insitutions requires URLs to be different for every investor as they might be cached at some point. Some information cannot be displayed by mistake and again, this is a legal requirement.
3. Think about content structure. note: some pages are available for all investors, some of them for specific investor. Let’s stick to these 2 cases only. Investor type should be applied to the URL.
4. Think about user experience. note: the solution should be easy to use and should leave minimal margin for an error. Ideally pages for specific investors should be completely separated, ticking a checkbox sounds like a too risky solution.

## Solution
The document must be written in English, contain at least 1500 characters, delivered in `.doc` or `.md` format. The task is estimated to 60 minutes of work.
