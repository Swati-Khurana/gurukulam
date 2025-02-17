---
title: 'Combinations'
date: 2018-11-14T19:02:50-07:00
draft: false
weight: 5
extensions:
    - katex
---




### வரிசை மாற்றங்கள் (Permutations)

வரிசை மாற்றம் என்றால் என்ன?

வரிசை மாற்றங்களை பல்வேறு சூழல்களில் எதிர்கொள்கிற�ோம்.

ூன்று நண்பர்கள் A , B மற்றும் C ஒரு புகைப்படம் எடுக்க வரிசையாக
நிற்கவேண்டும். எத்தனை விதமான வரிசைகளில் நிற்கலாம்? இவை இடமிருந்து
வலமாக கீழே தரப்பட்டுள்ளது.

A, B, C : A, C, B : B, A, C

B, C, A : C, A, B : C, B, A

ஆகவே, ம�ொத்தமாக புகைப்படம் எடுக்க 6 வழிகளில் தங்களுக்குள்
வரிசையாக நிற்க வைக்கலாம்.

ஆகவே, 3 ப�ொருட்களை ஒரு வரிசையில் அடுக்க \\(3 × 2×1 = 3!\\) வரிசை மாற்றங்கள் இருக்கும்.
நான்கு ப�ொருட்களை ஒரு சமயத்தில் எடுக்கும் ப�ோது கிடைக்கும் வரிசை மாற்றங்களின் எண்ணிக்கை
\\(4 × 3 ×2×1 = 4!\\)ஆகும். எனவே, ப�ொதுவாக n ப�ொருட்களை ஒரு வரிசையில் அடுக்க ம�ொத்தம்
\\( n ×(n-1)×(n-2)× ...×3×2×1 = n! \\)வரிசை மாற்றங்கள் இருக்கும்.

நம்மிடம் உள்ள A, B, C, D, E, F மற்றும் G என்ற 7 எழுத்துகளில் நாம் 4 எழுத்துகளை கொண்டு
எழுத்துச் சரங்களை உருவாக்கும் போது, முதல் எழுத்தினை தேர்ந்தெடுக்க நம்மிடம் 7 வழிகள்
உள்ளன. முதல் எழுத்தை தேர்ந்தெடுத்த பின்னர், நம்மிடம் இரண்டாம் இடத்திற்கு 6 எழுத்துகள்
உள்ளன. இதுபோல தொடர, 4 ஆவது எழுத்திற்கு 4 வாய்ப்புகள் உள்ளன.

எனவே, 7 எழுத்துகளில் இருந்து உருவாக்கப்படும் 4 எழுத்துச் சரங்களின் எண்ணிக்கை

\\( 7×6×5×4 = \frac{ 7×6×5×4×3×2×1}{3×2×1}\\) = \\(\frac{7!} {3!}\\) =\\(\frac{7!} {(7-4)!}\\)

பொதுவாக, n வெவ்வேறான பொருட்களில் இருந்து r பொருட்களை கொண்டு உருவாக்கும்
வரிசை மாற்றங்களின் எண்ணிக்கை \\(\frac{n!} {(n-r)!}\\) இதனை குறியீட்டால் \\(^nP_{r}\\) என குறிக்கலாம்.
இதற்கான முறையான நிரூபணத்தை இந்தப் பகுதியில் காண்போம்.

வெவ்வேறான பொருட்களின் மீதான வரிசை மாற்றங்கள் (Permutations of Distinct Objects)
சார்புகளின் வாயிலாக வரிசை மாற்றத்தை S = \\( \lbrace x_1,x_2...x_n\rbrace \\) என்ற முடிவுற்ற கணத்திலிருந்து S-ன் மீதே வரையறுக்கப்பட்ட ஓர் இருபுற சார்பை ஓர் வரிசை மாற்றம் என வரையறுக்கலாம். S-ன்
வரிசை மாற்றங்களின் எண்ணிக்கையும் S-ன் மீது வரையறுக்கப்பட்ட இருபுற சார்புகளின்
எண்ணிக்கையும் சமம்.

இந்த வரிசை மாற்றங்களின் எண்ணிக்கையை \\(^nP_{r}\\) என குறிக்கலாம்.

தேற்றம் 4.1
n, r ஆகியவை மிகை முழு எண்கள் மேலும் \\( r \le n\\) எனில், n வெவ்வேறான பொருட்களில்
இருந்து ஒரு சமயத்தில் r பொருட்களை கொண்டு உருவாக்கும் வரிசை மாற்றங்களின் எண்ணிக்கை
\\( n (n-1)(n-2)...(n-r+1) \\)ஆகும்.

நிரூபணம் ஒரு வரிசை மாற்றம் என்பது வரிசையில் அமைத்தலாகும். n வெவ்வேறான
பொருட்களிலிருந்து ஒரு சமயத்தில் r பொருட்களை கொண்டு உருவாக்கும் வரிசை மாற்றத்தினை,
n பொருட்களை r இடங்களில் அமைத்து பெறலாம்.






முதல் இடத்தை நிரப்ப n பொருட்கள் உள்ளன இரண்டாவது இடத்தை நிரப்புவதற்கு n - 1
பொருட்கள் உள்ளன. மூன்றாம் இடத்தை நிரப்ப n - 2 பொருட்கள் உள்ளன. இதுபோல கடைசி வரை
தொடர, அதாவது r ஆவது இடத்தை நிரப்ப (n - (r - 1)) பொருட்கள் உள்ளன. பெருக்கல் விதியின்
படி நாம் \\( ^nP_r \\) = n(n - 1)(n - 2)...(n - r + 1) எனப் பெறலாம்.

#### தேற்றம் 4.2

\\(n \ge 1 \\) மற்றும்\\( 0 \le r \le n\\)  எனில் \\(^nP_{r}\\) = \\(\frac{n!} {(n-r)!}\\)

நிரூபணம் தேற்றம் 4.1 -லிருந்து,

 \\( ^nP_r \\) = n×(n - 1)×(n - 2)×...×(n - r + 1)
 
 =  \\( \  {n×(n - 1)×(n - 2)×...×(n - r + 1)×(n-r)×(n-r-1)×...×2×1} {(n-r)×(n-r-1)×...×2×1}\\)

 =   \\(\frac{n!} {(n-r)!}\\),

