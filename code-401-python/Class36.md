# Data Fetching

## Reading:
#### What is SWR?
- SWR stands for stale-while-revalidate, a HTTP cache invalidation strategy popularized by HTTP RFC 5861.
- SWR is created by Vercel and one of its advantages is that it is a fast and lightweight package. It is a layer built on top of Fetch API and therefore provides additional features on top of just data fetching. These features include caching, pagination, auto revalidation and more.

#### Steps 
- Returns cached data first (stale)
- Sends the fetch request (revalidate)
- Returns the up-to-date data

#### Why use SWR?
1. Built-in Cache + Real-Time Experience
2. Auto Revalidation
3. Pagination
4. More Features + Benefits of SWR


#### Features of SWR
- Fast, lightweight and reusable data fetching
- Built-in cache and request deduplication
- Real-time experience
- Transport and protocol agnostic
- SSR / ISR / SSG support
- TypeScript ready
- React Native