## Hi there 👋

<!--
**SaguAM123/SaguAM123** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
This function is to check
// if a given number is prime
bool isPrime(int n)
{
    // 0 and 1 are not prime numbers
    if (n == 1 || n == 0)
        return false;

    // Check for divisibility from 2 to sqrt(n)
    for (int i = 2; i <= sqrt(n); i++) {
        if (n % i == 0)
            return false;
    }
    return true;
}

// Driver code
int main()
{
    int N = 50;

    // Check every number from 1 to N
    for (int i = 1; i <= N; i++) {
        if (isPrime(i)) {
            printf("%d ", i);
        }
    }

    return 0;
}
