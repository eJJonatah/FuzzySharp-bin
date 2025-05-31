> [!IMPORTANT]
> Please note that this is a fork from [FuzzySharp](https://github.com/JakeBayer/FuzzySharp) and does not contains the source code, the only purpose of it 
is to provide the compiled binaries of the original code, for both win and linux in x64 architecture. I DO NOT OWN THIS CODE and its licensed
by [@JakeBayer](https://github.com/JakeBayer) with the standart MIT License. The Compiled binaries are from the version under the next commit id
53b71acd66e53a4ff9f4229348de48295f99c0a5


# FuzzySharp
C# .NET fuzzy string matching implementation of Seat Geek's well known python FuzzyWuzzy algorithm. 

# Release Notes:
v.2.0.0

As of 2.0.0, all empty strings will return a score of 0. Prior, the partial scoring system would return a score of 100, regardless if the other input had correct value or not. This was a result of the partial scoring system returning an empty set for the matching blocks As a result, this led to incorrrect values in the composite scores; several of them (token set, token sort), relied on the prior value of empty strings.

As a result, many 1.X.X unit test may be broken with the 2.X.X upgrade, but it is within the expertise fo all the 1.X.X developers to recommednd the upgrade to the 2.X.X series regardless, should their version accommodate it or not, as it is closer to the ideal behavior of the library.


## Usage

Download the artifacts from your specific platform and import them to your project
