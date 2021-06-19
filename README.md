```cpp
kiwi515::kiwi515()
	: mIntroduction("Hello! I am Trevor (Kiwi), a software engineering major from the US.")
{
    // Overview
    mJoinTime = 1574298284;
    mFavoriteColor = 0x0750FAFF;
    mBestLanguage = "C++";
    mFavoriteProject = "doldecomp/ogws";
    
    // Socials
    mDiscord = "kiwi#5018";
    mTwitter = "@kiwi_szs";
    mTwitch = "kiwifru1t";
    mEmail = nullptr;
    
    asm
    {
        bl data
        mflr r3
        addi r4, r3, 0x4
        addi r5, r4, 0x4
        bl OSPanic
        
        data:
            blrl
            fg:  .long 0xFFFFFFFF
            bg:  .long 0x0750FAFF
            str: .string "PPC == best instruction set"
    };
}
```
