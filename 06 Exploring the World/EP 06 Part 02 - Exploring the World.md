## Data Fetching

<img width="1397" height="488" alt="image" src="https://github.com/user-attachments/assets/7d5b858a-292d-4a74-bd3f-58a2ff5063c4" />

In React, we will always be using the **second approach.** It gives us a **better UX.**

In the first method, till the API call (500ms), our page is frozen. And after 500ms, we suddenly see everything. This is a **"Poor UX"**

Instead, in the second approad, we render the **skeleton.** At the first, we can see here something and slowly, the websites loads. It's a **Better User Experience (UX)** and user doesn't face any lag or jitterinesh.

We can observe, we are rendering twice in the second approach, but the pro of using React is that it's render cycle is very fast. React render's the UI very fast. So, we don't have to bother much about, how much we are rendering (We bother abot rendering, but 2 renders are okay).

So, in React, we will follow the **Second Approach.**
