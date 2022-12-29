**Bad shuffling.** Suppose that you choose a random integer between 0 and n-1 in our shuffling code instead of one between i and n-1. Show that the resulting order is not equally likely to be one of the n! possibilities. Run the test of the previous exercise for this version.
Partial solution: when n = 3, all 3! = 6 outcomes are possible, but some are more likely:

![Screenshot (2053)](https://user-images.githubusercontent.com/90744289/208138044-1d1e95b3-8bc9-47dc-b7fa-dc3b75d79f3f.png)

Here's what happened to [PlanetPoker](https://www.datamation.com/entdev/article.php/616221/How-We-Learned-to-Cheat-at-Online-Poker-A-Study-in-Software-Security.htm) when they used a broken shuffling algorithm that could only generate only about 200,000 of the possible 52! shuffles.
