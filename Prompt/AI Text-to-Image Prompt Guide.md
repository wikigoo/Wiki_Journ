# **The Complete Guide to Professional Text-to-Image Prompting**

## _A Practical Manual for Journalists and Content Creators_

---

## **PART I: FOUNDATIONS**

### **Chapter 1: Understanding AI Image Generation**

#### 1.1 How AI Interprets Your Words

When you type a prompt into an AI image generator, you're not communicating with an intelligent entity that "understands" your intent. Instead, you're providing coordinates in a vast mathematical space where the AI has learned to associate certain word patterns with visual outcomes.

**The Statistical Nature of AI Understanding:**

AI models like DALL-E 3, Midjourney, and Stable Diffusion are trained on billions of image-text pairs scraped from the internet. When you write "a confident politician," the AI doesn't understand "confidence" as an emotion. Instead, it statistically correlates that phrase with images tagged similarly in its training data - typically showing people with upright posture, direct eye contact, and formal attire.

**Why This Matters for Journalists:**

Understanding this statistical foundation is crucial because it explains why:

- Specific terms yield better results than abstract concepts
- Cultural biases appear in outputs (Western defaults for "politician" or "journalist")
- Certain combinations of words create unexpected visual results
- Consistency requires identical or very similar phrasing

**Practical Application:**

Instead of writing: "A successful leader addressing the nation" Write: "A middle-aged political leader in formal dark suit standing at wooden podium with national flag background, confident upright posture, direct eye contact with camera, professional studio lighting"

#### 1.2 The Generation Process Explained

**From Words to Numbers (Text Encoding):**

Your prompt undergoes several transformations:

1. **Tokenization**: Words are broken into smaller units
2. **Embedding**: Each token becomes a numerical vector
3. **Conditioning**: These vectors guide the image generation process

**The Diffusion Process:**

Modern AI image generators use a process called diffusion:

1. **Start with noise**: A field of random static pixels
2. **Iterative refinement**: The AI gradually removes noise over 20-50 steps
3. **Text guidance**: Your prompt's numerical representation guides each step
4. **Final decode**: The result is converted back to visible pixels

**Seeds and Reproducibility:**

Every generation starts with a "seed" - a number that determines the initial noise pattern. Using the same seed with identical prompts produces identical images, making this crucial for:

- Creating variations of the same concept
- Maintaining consistency across a series
- Reproducing successful results

**Platform Differences:**

- **DALL-E 3**: Optimized for natural language, integrated with ChatGPT for conversational refinement
- **Midjourney**: Emphasizes artistic quality, uses Discord interface with parameter system
- **Stable Diffusion**: Open-source, maximum customization, steep learning curve

#### 1.3 Common Limitations and Expectations

**Anatomical Accuracy Challenges:**

AI struggles with:

- **Hands and fingers**: Often produces wrong number of digits or unnatural poses
- **Facial symmetry**: Eyes may be uneven, teeth distorted
- **Complex poses**: Multiple people interacting, unusual positions

**Solutions for Journalists:**

- Use negative prompts: "ugly, deformed hands, extra fingers, asymmetrical eyes"
- Specify: "detailed hands, symmetrical face, natural pose"
- Choose simpler compositions when accuracy is critical

**Text Rendering Capabilities:**

Most AI models cannot reliably render readable text except DALL-E 3. For news graphics requiring text:

- **DALL-E 3**: Can create headlines, banners, simple graphics with text
- **Others**: Generate image, add text in post-production
- **Workaround**: Describe text placement, add actual text later

**Cultural Bias in Training Data:**

AI models reflect biases in their training data:

- "Politician" often defaults to older white men
- "Journalist" may show Western stereotypes
- Middle Eastern representations may rely on outdated or stereotypical imagery

**Mitigation Strategies:**

- Be explicit about demographics: "Iranian female journalist in hijab"
- Specify cultural context: "Persian architectural background"
- Use diverse reference descriptors

**Managing Realistic Expectations:**

AI excels at:

- Creating variations quickly
- Generating concepts for brainstorming
- Producing high-quality single subjects
- Mixing styles and concepts creatively

AI struggles with:

- Perfect accuracy in complex scenes
- Specific real people (ethically restricted)
- Precise historical accuracy
- Fine text details

### **Chapter 2: The Universal Prompt Formula**

#### 2.1 The Three-Layer Structure

Every effective prompt follows a hierarchical structure that mirrors how AI processes information:

**Layer 1: Subject & Scene (WHO + WHAT + WHERE)**

This foundation layer establishes the core content. Place this first because AI gives highest weight to initial words.

_Components:_

- **Primary Subject**: The main focus (person, object, concept)
- **Action/State**: What the subject is doing or how they appear
- **Environment**: Where the scene takes place
- **Context**: Time period, situation, atmosphere

_Example:_ "Iranian foreign minister in formal diplomatic attire sitting at negotiation table in modern conference room"

**Layer 2: Style & Medium (HOW IT LOOKS)**

This layer defines the aesthetic approach and visual treatment.

_Components:_

- **Medium**: Photography, painting, digital art, sketch
- **Artistic style**: Photorealistic, documentary, editorial, artistic
- **Historical reference**: Art movements, photographer styles
- **Mood**: Professional, dramatic, intimate, authoritative

_Example:_ "professional diplomatic photography style, documentary realism, natural conference room lighting"

**Layer 3: Technical Quality (PROFESSIONAL STANDARDS)**

This final layer ensures professional output quality.

_Components:_

- **Resolution**: 8K, UHD, high detail
- **Camera specs**: Lens type, shot composition
- **Quality boosters**: Professional, award-winning, masterpiece
- **Technical details**: Sharp focus, proper exposure

_Example:_ "shot with 85mm lens, shallow depth of field, professional photography, 8K detail, sharp focus"

**Complete Formula Example:** "Iranian foreign minister in formal diplomatic attire sitting at negotiation table in modern conference room, professional diplomatic photography style, documentary realism, natural conference room lighting, shot with 85mm lens, shallow depth of field, professional photography, 8K detail, sharp focus"

#### 2.2 Prompt Order and Weight

**Why Sequence Matters:**

AI attention mechanisms assign decreasing importance to words as they appear later in prompts. Critical elements should appear early.

**Optimal Order:**

1. **Primary subject** (first 3-5 words)
2. **Key descriptors** (next 10-15 words)
3. **Setting and context** (middle section)
4. **Style and mood** (latter portion)
5. **Technical specifications** (end)

**Weight Distribution Examples:**

_High Impact Opening:_ "Presidential candidate during televised debate..."

_Medium Impact Middle:_ "...standing at podium in television studio with blue backdrop..."

_Low Impact Ending:_ "...professional broadcast lighting, 8K, shot with professional camera"

**Balancing Specificity with Flexibility:**

Too specific: "45-year-old Iranian politician with exactly three wrinkles wearing navy blue suit with red tie standing at brown wooden podium"

Too vague: "A person talking"

Optimal: "Middle-aged Iranian political leader in formal attire addressing audience from parliamentary podium"

### **Chapter 3: Platform Overview and Selection**

#### 3.1 DALL-E 3: Conversational and Safe

**Core Strengths:**

- **Natural language processing**: Understands complex, conversational prompts
- **Text integration**: Only platform reliable for readable text in images
- **Safety filters**: Appropriate for public figures and sensitive content
- **ChatGPT integration**: Iterative refinement through conversation

**Best Applications for Journalism:**

- News graphics with headlines or text
- Public figure representations (with restrictions)
- Infographic-style content
- Social media graphics requiring text

**Practical Workflow:**

1. Start with conversational prompt in ChatGPT
2. Request specific changes through dialogue
3. Refine until result meets requirements
4. Export final image

**Example Workflow:**

```
User: "Create a news graphic showing economic growth in Iran"
ChatGPT: [Generates initial image]
User: "Make the chart more prominent and add Persian text"
ChatGPT: [Refines image with adjustments]
User: "Change the color scheme to match our brand colors"
ChatGPT: [Final version with brand alignment]
```

**Limitations:**

- Less artistic control than competitors
- Safety restrictions may block legitimate news content
- Cannot generate specific real people
- Limited parameter customization

#### 3.2 Midjourney: Artistic and Cinematic

**Core Strengths:**

- **Visual aesthetics**: Produces consistently beautiful, cinematic results
- **Consistency tools**: --cref and --sref for character and style matching
- **Parameter control**: Fine-tuning through command-line style parameters
- **Community**: Large user base sharing techniques and styles

**Key Parameters for Journalists:**

**Aspect Ratio (--ar):**

- `--ar 16:9`: Widescreen for video thumbnails, web headers
- `--ar 9:16`: Vertical for mobile, Instagram stories
- `--ar 1:1`: Square for social media posts
- `--ar 3:2`: Standard photography ratio

**Stylize (--stylize or --s):**

- `--s 0`: Maximum prompt adherence, minimal artistic interpretation
- `--s 50`: Balanced approach, good for journalism
- `--s 100`: Default Midjourney aesthetic
- `--s 250+`: Highly artistic, less literal

**Character Reference (--cref):**

```
/imagine [prompt] --cref [image_URL] --cw 80
```

- Maintains character consistency across multiple images
- --cw controls strength (0-100)

**Style Reference (--sref):**

```
/imagine [prompt] --sref [image_URL] --sw 50
```

- Applies visual style from reference image
- --sw controls style strength (0-1000)

**Practical Journalism Workflow:**

1. Generate initial concept with basic prompt
2. Use --cref for character consistency in multi-image stories
3. Apply --sref for brand-consistent styling
4. Adjust --stylize for appropriate realism level

**Example for Political Coverage:**

```
/imagine Iranian parliament session with legislators in formal debate, documentary photography style, natural lighting --ar 16:9 --s 25 --q 2
```

#### 3.3 Stable Diffusion: Technical and Customizable

**Core Strengths:**

- **Maximum control**: Detailed parameter adjustment
- **Custom models**: Specialized checkpoints for specific needs
- **Negative prompts**: Precise exclusion control
- **Open source**: Community innovations and modifications

**Essential Parameters:**

**CFG Scale (Classifier-Free Guidance):**

- 1-6: High creativity, loose prompt adherence
- 7-12: Balanced approach (recommended for journalism)
- 13-20: Strict adherence, may cause artifacts

**Sampling Steps:**

- 20-30: Fast generation, good quality
- 30-50: Higher quality, slower
- 50+: Diminishing returns

**Negative Prompts:** Essential for quality control:

```
Negative: ugly, deformed, disfigured, poorly drawn hands, extra fingers, mutated hands, poorly drawn face, bad anatomy, blurry, low quality, worst quality, jpeg artifacts, watermark, signature, text, amateur, distorted
```

**Advanced Techniques:**

**Prompt Weighting:**

- `(important concept:1.3)`: Increase emphasis
- `[less important:0.8]`: Decrease emphasis
- `((very important:1.5))`: Strong emphasis

**Custom Models for Journalism:**

- **Realistic Vision**: Excellent for photorealism
- **Deliberate**: Balanced realism and artistry
- **epiCRealism**: Professional photography style

**Practical Workflow:**

1. Choose appropriate checkpoint model
2. Craft detailed positive prompt
3. Include comprehensive negative prompt
4. Set CFG scale 7-9 for journalism
5. Use 25-35 sampling steps
6. Generate multiple variations
7. Upscale best results

---

## **PART II: VISUAL MASTERY**

### **Chapter 4: Lighting and Atmosphere Control**

#### 4.1 Professional Lighting Techniques

**Portrait Lighting for News Figures:**

**Three-Point Lighting Setup:** The foundation of professional photography, easily replicated in AI prompts:

```
"Professional three-point lighting setup with key light from 45-degree angle, soft fill light reducing shadows, and subtle back light for separation"
```

**Rembrandt Lighting:** Creates dramatic, authoritative mood perfect for serious political coverage:

```
"Rembrandt lighting with strong key light creating characteristic triangle of light on shadowed cheek, dramatic shadows, professional portrait style"
```

**Butterfly Lighting:** Flattering for formal portraits and official imagery:

```
"Butterfly lighting with high front key light creating small shadow under nose, even facial illumination, formal portrait style"
```

**Natural vs. Studio Lighting:**

_For Documentary Realism:_

```
"Natural window lighting, soft diffused daylight, candid documentary style, authentic atmosphere"
```

_For Official Portraits:_

```
"Professional studio lighting, controlled illumination, softbox lighting, formal presentation, executive portrait style"
```

**Atmospheric Lighting Applications:**

**Golden Hour for Emotional Impact:**

```
"Golden hour lighting casting warm amber glow, long soft shadows, emotional warmth, inspiring atmosphere"
```

**Blue Hour for Serious Topics:**

```
"Blue hour twilight lighting, cool professional tones, serious atmosphere, contemplative mood"
```

**Dramatic News Coverage:**

```
"Harsh directional lighting, strong contrast shadows, dramatic atmosphere, breaking news urgency"
```

#### 4.2 Cultural Context Lighting

**Appropriate Lighting for Iranian Cultural Content:**

**Religious and Ceremonial Settings:**

```
"Respectful soft lighting appropriate for mosque interior, warm traditional ambiance, cultural sensitivity, reverent atmosphere"
```

**Government and Official Settings:**

```
"Formal governmental lighting, official parliamentary ambiance, dignified professional illumination, institutional gravitas"
```

**Traditional vs. Modern Balance:**

```
"Balanced lighting showing modern Iranian progress while respecting traditional values, contemporary yet culturally appropriate"
```

**Regional and Seasonal Considerations:**

**Desert and Arid Region Lighting:**

```
"Bright clear desert lighting, intense sunlight balanced with strategic shadows, Middle Eastern atmospheric clarity"
```

**Urban Persian Architecture:**

```
"Architectural lighting emphasizing traditional Persian design elements, respectful cultural presentation, historical significance"
```

#### 4.3 Technical Lighting Specifications

**Color Temperature Control:**

**Warm Light (2700K-3200K):** Applications: Intimate interviews, cultural events, emotional stories

```
"Warm tungsten lighting, cozy amber glow, intimate atmosphere, emotional warmth"
```

**Neutral Daylight (5000K-5600K):** Applications: News reporting, official events, factual coverage

```
"Neutral daylight balance, accurate color reproduction, professional news lighting, clear visibility"
```

**Cool Light (6000K-7000K):** Applications: Technology stories, modern settings, corporate coverage

```
"Cool professional lighting, modern corporate atmosphere, clean contemporary feel, technological precision"
```

**Directional Lighting for Different Moods:**

**Authoritative and Powerful:**

```
"Low-angle dramatic lighting, upward shadows, powerful authoritative presence, leadership gravitas"
```

**Approachable and Trustworthy:**

```
"Gentle front lighting, minimal shadows, approachable demeanor, trustworthy presentation"
```

**Serious and Contemplative:**

```
"Side lighting with controlled shadows, thoughtful atmosphere, serious consideration, depth of character"
```

### **Chapter 5: Composition and Camera Control**

#### 5.1 News Photography Composition

**Shot Types for Different Journalism Scenarios:**

**Wide Establishing Shots:** Perfect for showing context, crowd sizes, environmental impact:

```
"Wide establishing shot showing full context of protest gathering in city square, environmental storytelling, documentary perspective, comprehensive scene coverage"
```

**Medium Shots for Interviews:** Balances subject and environment, standard for news interviews:

```
"Medium shot framing subject from waist up, professional interview composition, balanced subject and background, standard journalism framing"
```

**Close-ups for Emotional Impact:** Emphasizes facial expressions and emotional content:

```
"Close-up portrait focusing on facial expression, emotional storytelling, intimate connection with viewer, detailed human interest"
```

**Overhead Views for Data Visualization:** Excellent for showing patterns, crowd sizes, or geographic context:

```
"Overhead drone perspective showing scale and organization of event, bird's eye view for comprehensive coverage, geographic context"
```

**Camera Angles and Their Psychological Impact:**

**Eye-Level for Neutral Reporting:** Most common for unbiased news presentation:

```
"Eye-level perspective maintaining neutral journalistic stance, unbiased viewpoint, standard news photography angle"
```

**Low Angles for Authority:** Makes subjects appear more powerful and authoritative:

```
"Low-angle shot emphasizing authority and leadership, powerful perspective, commanding presence"
```

**High Angles for Context:** Shows vulnerability or provides broader perspective:

```
"High-angle perspective providing broader context, comprehensive view of situation, environmental overview"
```

#### 5.2 Professional Framing Techniques

**Rule of Thirds Implementation:**

**For Single Subjects:**

```
"Composition following rule of thirds with subject positioned on right vertical line, balanced visual weight, professional photography standards"
```

**For Environmental Storytelling:**

```
"Rule of thirds composition with horizon on lower third line, subject on left intersection point, environmental context in upper two-thirds"
```

**Leading Lines for Visual Flow:**

**Architectural Leading Lines:**

```
"Leading lines from architectural elements drawing eye to main subject, directional visual flow, structured composition"
```

**Natural Leading Lines:**

```
"Natural leading lines from pathway/river/shoreline guiding viewer attention to focal point, organic visual progression"
```

**Depth of Field for Focus Control:**

**Shallow Depth for Subject Isolation:**

```
"Shallow depth of field with subject in sharp focus, background softly blurred, professional portrait technique, subject isolation"
```

**Deep Depth for Environmental Context:**

```
"Deep depth of field keeping entire scene in sharp focus, comprehensive environmental detail, landscape photography style"
```

#### 5.3 Aspect Ratio Optimization

**16:9 for Digital Media:** Standard for web headers, video thumbnails, presentation slides:

```
"Widescreen 16:9 composition optimized for digital display, horizontal format maximizing screen real estate"
```

**9:16 for Mobile and Social:** Vertical format for Instagram stories, mobile viewing:

```
"Vertical 9:16 composition optimized for mobile viewing, portrait orientation for social media platforms"
```

**1:1 for Social Media Posts:** Square format for Instagram feeds, balanced composition:

```
"Square 1:1 composition with centered subject, balanced visual weight for social media posting"
```

**Custom Ratios for Print:** Traditional newspaper and magazine formats:

```
"3:2 aspect ratio for traditional print media, classic photography proportions, editorial layout compatibility"
```

### **Chapter 6: Style and Cultural Adaptation**

#### 6.1 Photorealistic News Style

**Documentary Realism Approach:**

The foundation of credible journalism imagery:

```
"Documentary photography style, natural lighting, candid authentic moment, journalistic integrity, real-world authenticity, unposed natural behavior"
```

**Key Characteristics:**

- Natural, available lighting
- Authentic, unposed moments
- Environmental storytelling
- Minimal artistic manipulation
- Focus on factual representation

**Applications:**

- Breaking news coverage
- On-location reporting
- Social issue documentation
- Political event coverage

**Editorial Photography Style:**

For feature stories and magazine-style content:

```
"Editorial photography style, controlled professional lighting, carefully composed but natural-looking, high production value, magazine quality"
```

**Key Characteristics:**

- Controlled but natural lighting
- Carefully planned composition
- Higher production value
- Polished but authentic feel
- Suitable for covers and features

**Applications:**

- Political profiles
- Economic analysis features
- Cultural coverage
- In-depth investigations

#### 6.2 Cultural Sensitivity in Style

**Iranian Context Considerations:**

**Appropriate Dress Codes:**

```
"Respectful representation following Iranian cultural dress standards, modest professional attire, culturally appropriate presentation"
```

**Religious and Cultural Symbols:**

```
"Respectful inclusion of Islamic cultural elements, appropriate religious symbolism, cultural sensitivity in representation"
```

**Traditional vs. Modern Balance:**

```
"Contemporary Iranian context while honoring traditional values, modern progress with cultural respect, balanced representation"
```

**International Figure Representation:**

**Avoiding Stereotypes:**

```
"Neutral diplomatic representation avoiding cultural stereotypes, respectful international coverage, unbiased visual presentation"
```

**Cross-Cultural Sensitivity:**

```
"Culturally aware international representation, diplomatic neutrality, respectful cross-cultural coverage"
```

#### 6.3 Genre-Specific Styles

**Political Reporting Aesthetics:**

**Parliamentary Coverage:**

```
"Formal parliamentary photography style, institutional dignity, governmental gravitas, official proceedings documentation"
```

**Campaign Coverage:**

```
"Dynamic campaign photography, energetic political atmosphere, public engagement, democratic process documentation"
```

**Diplomatic Events:**

```
"Formal diplomatic photography, international protocol appropriate, ceremonial dignity, state event documentation"
```

**Economic and Business Coverage:**

**Corporate Settings:**

```
"Professional business photography, corporate environment, executive presentation, economic authority"
```

**Market and Trade Coverage:**

```
"Commercial photography documenting economic activity, trade and commerce, market dynamics, business operations"
```

**Cultural Event Coverage:**

**Traditional Celebrations:**

```
"Cultural event photography respecting traditional celebrations, festive atmosphere, community gathering, cultural heritage"
```

**Arts and Literature:**

```
"Cultural arts photography, intellectual atmosphere, creative community, artistic achievement documentation"
```

---

## **PART III: TECHNICAL EXCELLENCE**

### **Chapter 7: Quality Enhancement and Detail Control**

#### 7.1 Professional Quality Boosters

**Resolution and Detail Keywords:**

Essential for professional output:

```
"8K UHD, ultra-high resolution, hyperdetailed, sharp focus, professional photography, award-winning quality, masterpiece, maximum detail"
```

**Camera Equipment References:**

These technical specifications signal professional quality:

```
"Shot on Canon EOS R5 with 85mm f/1.4 lens, professional DSLR photography, high-end camera equipment, commercial photography standards"
```

**Alternative Equipment References:**

- "Shot on Hasselblad medium format"
- "Leica M-series photography"
- "Sony A7R IV professional setup"
- "Nikon D850 with professional glass"

**Professional Photography Terminology:**

Industry-standard language that improves output quality:

```
"Professional photography, editorial quality, commercial photography standards, studio photography, professional lighting setup"
```

**Surface and Material Specifications:**

**Fabric and Clothing Details:**

```
"High-quality wool suit with fine weave texture, silk tie with subtle sheen, polished leather shoes, professional tailoring details"
```

**Architectural Materials:**

```
"Polished marble surfaces, brushed steel fixtures, natural wood grain, premium construction materials"
```

**Skin and Human Details:**

```
"Natural skin texture, detailed facial features, authentic aging, individual character details, realistic human representation"
```

#### 7.2 Negative Prompting for Quality Control

**Universal Quality Filter:**

Essential negative prompt for all professional work:

```
Negative: ugly, deformed, disfigured, poorly drawn hands, extra fingers, mutated hands, poorly drawn face, bad anatomy, bad proportions, extra limbs, cloned face, malformed limbs, missing arms, missing legs, extra arms, extra legs, fused fingers, too many fingers, long neck, blurry, low quality, worst quality, jpeg artifacts, watermark, signature, text, amateur, distorted, asymmetrical eyes
```

**Platform-Specific Applications:**

**Stable Diffusion Comprehensive Negative:**

```
Negative: ugly, tiling, poorly drawn hands, poorly drawn feet, poorly drawn face, out of frame, extra limbs, disfigured, deformed, body out of frame, bad anatomy, watermark, signature, cut off, low contrast, underexposed, overexposed, bad art, beginner, amateur, distorted face, blurry, draft, grainy
```

**Midjourney No Parameter:**

```
--no ugly, deformed, blurry, amateur, low quality, watermark
```

**Style Exclusion Techniques:**

**For Photorealism:**

```
Negative: painting, illustration, drawing, art, sketch, cartoon, anime, cgi, 3d, rendered
```

**For Serious News Content:**

```
Negative: cartoon, comic, funny, humorous, exaggerated, caricature, satirical
```

#### 7.3 Advanced Parameter Control

**Stable Diffusion CFG Scale Optimization:**

**For Journalism (Recommended: 7-9):**

- CFG 7: Slight creative interpretation, natural results
- CFG 8: Balanced adherence and quality
- CFG 9: Strong prompt following, detailed results

**Sampling Methods for News:**

- **DPM++ 2M Karras**: Fast, high quality, good for deadlines
- **Euler A**: Reliable, consistent results
- **DDIM**: Predictable, good for batch generation

**Midjourney Parameter Combinations:**

**For News Photography:**

```
--stylize 25 --chaos 10 --quality 2
```

**For Editorial Features:**

```
--stylize 50 --chaos 20 --quality 2
```

**For Breaking News (Speed Priority):**

```
--stylize 15 --chaos 5 --quality 1 --fast
```

### **Chapter 8: Consistency and Character Control**

#### 8.1 Political Figure Consistency

**Character Description Templates:**

**Template for Government Officials:**

```
[Age] Iranian [position] with [hair description], wearing [attire description], [facial features], [expression], in [setting], [lighting], [style specifications]
```

**Example Application:**

```
"Middle-aged Iranian foreign minister with graying hair and beard, wearing dark formal diplomatic suit, dignified facial features with kind eyes, confident professional expression, in modern conference room, natural professional lighting, documentary photography style, 8K detail"
```

**Consistency Maintenance Techniques:**

**Seed Locking Method:**

1. Generate initial character with detailed prompt
2. Note the seed number
3. Use identical seed for variations
4. Modify only action/setting words
5. Maintain core character description

**Reference Image Method (Midjourney):**

```
/imagine [new scenario] --cref [original_image_URL] --cw 80
```

**Character Weight Settings:**

- --cw 100: Complete character match
- --cw 80: Strong character similarity (recommended)
- --cw 60: Moderate character influence
- --cw 40: Loose character reference

#### 8.2 Environmental and Setting Consistency

**Government Building Templates:**

**Parliamentary Setting:**

```
"Iranian parliament chamber with curved seating arrangement, formal wooden panels, national emblems, official governmental atmosphere, formal institutional lighting"
```

**Diplomatic Meeting Room:**

```
"Modern diplomatic conference room with long polished table, formal chairs, international flags, professional meeting atmosphere, neutral diplomatic setting"
```

**Press Conference Setup:**

```
"Official press conference setting with podium, microphones, media backdrop, professional lighting, governmental press room atmosphere"
```

**Maintaining Visual Continuity:**

**Style Reference Method (Midjourney):**

```
/imagine [new content] --sref [setting_reference_URL] --sw 60
```

**Template Substitution:**

1. Create master environmental description
2. Save as template with variables
3. Substitute only subject/action elements
4. Maintain environmental constants

### **Chapter 9: Advanced Parameter Control**

#### 9.1 Platform-Specific Optimization

**Midjourney Advanced Workflows:**

**News Photography Preset:**

```
/imagine [prompt] --ar 16:9 --stylize 25 --chaos 15 --quality 2 --version 6
```

**Editorial Feature Preset:**

```
/imagine [prompt] --ar 3:2 --stylize 40 --chaos 25 --quality 2 --version 6
```

**Social Media Preset:**

```
/imagine [prompt] --ar 1:1 --stylize 35 --chaos 20 --quality 2 --version 6
```

**Stable Diffusion News Optimization:**

**Standard News Generation:**

```
Steps: 30
CFG Scale: 8
Sampler: DPM++ 2M Karras
Resolution: 1024x1024 (then upscale)
Clip Skip: 1
```

**Batch News Production:**

```
Steps: 25 (faster)
CFG Scale: 7
Sampler: Euler A
Batch Count: 4
```

#### 9.2 Batch Production and Scaling

**Template-Based Workflows:**

**Master Template Structure:**

```
[SUBJECT_VAR] + [CONSISTENT_STYLE] + [CONSISTENT_QUALITY] + [CONSISTENT_TECHNICAL]
```

**Example Implementation:**

```
Template: "{subject} in formal diplomatic setting, professional photography, natural lighting, 8K detail, sharp focus"

Variables:
- Iranian foreign minister
- Economic advisor  
- Parliamentary speaker
- Cultural attaché
```

**Quality Control at Scale:**

**Three-Stage Review Process:**

1. **Rapid Triage** (30 seconds per image)
    
    - Obvious technical failures
    - Anatomical deformities
    - Completely off-prompt results
2. **Content Review** (2 minutes per image)
    
    - Cultural appropriateness
    - Professional standards
    - Brand alignment
3. **Final Polish** (5 minutes per image)
    
    - Minor detail corrections
    - Color/contrast adjustments
    - Format optimization

---

## **PART IV: PROFESSIONAL APPLICATION**

### **Chapter 10: Journalism-Specific Workflows**

#### 10.1 Breaking News Visual Creation

**Rapid Response Protocol:**

**Time-Critical Situation (Under 30 minutes):**

1. **Platform Selection**: DALL-E 3 for speed and safety
2. **Template Activation**: Use pre-written prompt templates
3. **Single Generation**: Accept first good result
4. **Minimal Post-Processing**: Basic cropping and format conversion

**30-Minute Breaking News Template:**

```
"Breaking news scene showing [situation] in [location], professional news photography, dramatic lighting, journalistic documentary style, urgent atmosphere, 8K quality"
```

**Examples:**

```
"Breaking news scene showing emergency response at government building in Tehran, professional news photography, dramatic lighting, journalistic documentary style, urgent atmosphere, 8K quality"

"Breaking news scene showing diplomatic meeting between international leaders, professional news photography, formal lighting, journalistic documentary style, serious atmosphere, 8K quality"
```

**2-Hour Response Protocol:**

1. **Platform**: Midjourney for higher quality
2. **Multiple Generations**: Create 3-4 options
3. **Client Review**: Quick approval process
4. **Basic Enhancement**: Color correction, minor edits

**Same-Day Response Protocol:**

1. **Platform**: Stable Diffusion for maximum control
2. **Comprehensive Generation**: Multiple angles and approaches
3. **Full Enhancement**: Complete post-processing workflow
4. **Multiple Formats**: Various sizes and orientations

#### 10.2 Feature Story Development

**Multi-Image Story Sequences:**

**Character Consistency Across Series:**

**Step 1: Establish Master Character**

```
"Distinguished Iranian economist in formal business attire, middle-aged with graying beard, intelligent expression, professional demeanor, detailed character study, 8K portrait"
```

**Step 2: Generate Seed Image** Save seed number and character description

**Step 3: Create Situation Variations**

```
Same character description + ", presenting economic data to parliament"
Same character description + ", reviewing documents in office"  
Same character description + ", meeting with international delegates"
```

**Environmental Storytelling Sequence:**

**Economic Growth Story Example:**

1. **Wide establishing shot**: Modern Tehran skyline
2. **Medium shot**: Busy financial district
3. **Close-up**: Market activity details
4. **Portrait**: Economic expert analysis

**Narrative Arc Development:**

**Three-Act Visual Structure:**

- **Setup**: Establish context and characters
- **Development**: Show action and change
- **Resolution**: Conclude with outcome/impact

#### 10.3 Social and Political Coverage

**Sensitive Topic Visualization:**

**Protest and Demonstration Coverage:**

**Balanced Perspective Approach:**

```
"Peaceful demonstration in public square, diverse crowd of citizens, respectful documentation, democratic expression, balanced journalistic perspective, natural lighting, documentary photography"
```

**Multiple Viewpoint Generation:**

1. Wide crowd shots for scale
2. Individual participant portraits
3. Official response documentation
4. Environmental impact views

**International Relations Coverage:**

**Diplomatic Meeting Visualization:**

```
"Formal diplomatic meeting between Iranian and international representatives, respectful bilateral discussion, professional conference setting, neutral diplomatic photography, balanced representation"
```

**Cultural Sensitivity Protocols:**

**Pre-Generation Checklist:**

- [ ] Culturally appropriate attire
- [ ] Respectful religious considerations
- [ ] Accurate geographic context
- [ ] Balanced demographic representation
- [ ] Professional diplomatic tone

**Post-Generation Review:**

- [ ] No cultural stereotypes present
- [ ] Respectful representation of all parties
- [ ] Accurate cultural details
- [ ] Professional news standards met

### **Chapter 11: Post-Generation Enhancement**

#### 11.1 AI-Powered Editing Tools

**Inpainting for Correction:**

**Common Correction Scenarios:**

**Hand Repair Workflow:**

1. Identify problematic hands/fingers
2. Mask affected area
3. Use inpainting prompt: "natural human hands, correct anatomy, five fingers, realistic pose"
4. Generate multiple options
5. Select best result

**Facial Enhancement:**

1. Mask facial area requiring correction
2. Inpainting prompt: "symmetrical professional face, natural expression, detailed features"
3. Maintain lighting consistency
4. Preserve character identity

**Background Replacement:**

1. Mask entire background
2. New background prompt: "professional office setting, natural lighting, blurred background"
3. Ensure lighting matches subject
4. Maintain depth of field consistency

**Upscaling for Print Quality:**

**AI Upscaling Workflow:**

1. **Real-ESRGAN**: General purpose, good for photographs
2. **ESRGAN**: Sharp details, good for architecture
3. **SwinIR**: Balanced approach, good for faces
4. **Waifu2x**: Illustrations and graphics

**Print Requirements:**

- **Web**: 72-96 DPI, sRGB color space
- **Newspaper**: 200-300 DPI, CMYK color space
- **Magazine**: 300+ DPI, CMYK or sRGB
- **Large Format**: 150-200 DPI minimum

#### 11.2 Integration with Traditional Tools

**Adobe Photoshop Workflow:**

**Professional Enhancement Process:**

1. **Import AI-generated image**
2. **Color correction**: Levels, curves, color balance
3. **Sharpening**: Unsharp mask or smart sharpen
4. **Noise reduction**: Reduce grain and artifacts
5. **Format optimization**: Save for intended use

**Text and Graphics Overlay:**

**News Graphics Workflow:**

1. Generate background image with AI
2. Add headline text in Photoshop
3. Include news ticker or logo
4. Add data visualization if needed
5. Export in multiple formats

**Batch Processing for Deadlines:**

**Photoshop Actions for Efficiency:**

1. Create standard correction action
2. Include color grading for brand consistency
3. Add watermark/logo placement
4. Size and format optimization
5. Apply to multiple images simultaneously

### **Chapter 12: Quality Assurance and Ethics**

#### 12.1 Technical Quality Control

**Professional Standards Checklist:**

**Before Publication Review:**

- [ ] Resolution meets publication requirements
- [ ] No visible AI artifacts (wrong fingers, distorted faces)
- [ ] Color accuracy and consistency
- [ ] Proper aspect ratio for intended use
- [ ] Sharp focus where intended
- [ ] Professional lighting quality
- [ ] Cultural appropriateness verified
- [ ] Brand guidelines compliance

**Resolution Verification:**

- **Digital**: Minimum 1920x1080 for web headers
- **Print**: 300 DPI at final print size
- **Social Media**: Platform-specific requirements
- **Archive**: Maximum available resolution

**Color Management:**

- **Monitor calibration**: Regular color accuracy checks
- **Color space**: sRGB for web, CMYK for print
- **Brand consistency**: Match established color guidelines
- **Cultural sensitivity**: Appropriate color choices

#### 12.2 Ethical and Legal Considerations

**Copyright and Usage Rights:**

**Platform-Specific Terms:**

**DALL-E 3/OpenAI:**

- User owns generated images
- Cannot generate copyrighted characters
- Commercial use permitted with subscription
- No liability for copyright claims

**Midjourney:**

- Paid subscribers own generated images
- Free users have limited rights
- Commercial use permitted for subscribers
- User assumes copyright liability

**Stable Diffusion:**

- Open source, user owns outputs
- Model training data copyright unclear
- User assumes all liability
- Commercial use varies by hosting platform

**Risk Mitigation Strategies:**

1. **Significant human modification**: Substantial editing and transformation
2. **Original concept development**: Use AI as inspiration, not final product
3. **Multiple source combination**: Blend elements from various generations
4. **Legal consultation**: For high-stakes commercial use

**Cultural and Social Responsibility:**

**Bias Detection Protocol:**

1. **Demographic review**: Verify diverse representation
2. **Stereotype check**: Avoid cultural clichés
3. **Context appropriateness**: Ensure culturally sensitive settings
4. **Community feedback**: Test with cultural consultants

**Ethical Guidelines for News:**

- **Truthfulness**: Visual content supports factual reporting
- **Transparency**: Disclose AI generation when relevant
- **Respect**: Dignified representation of all subjects
- **Accuracy**: Visual elements align with story facts

---

## **PART V: PRACTICAL RESOURCES**

### **Chapter 13: Template Library and Examples**

#### 13.1 Government and Political Templates

**Parliamentary Session Coverage:**

```
Template: "Iranian parliamentary session with legislators in formal debate, {specific_action}, professional governmental photography, formal institutional lighting, documentary journalism style, respectful political coverage, 8K detail, 16:9 aspect ratio"

Variables:
- voting on important legislation
- discussing economic policy
- addressing national security
- debating social reforms
```

**Presidential/Official Portraits:**

```
Template: "Formal portrait of {position} in {setting}, dignified professional appearance, {attire}, confident leadership expression, official governmental photography, studio lighting, executive portrait style, 8K detail"

Variables:
Position: President, Minister, Ambassador, Speaker
Setting: presidential office, ministerial chamber, diplomatic venue
Attire: formal suit, traditional dress, diplomatic attire
```

**International Diplomacy:**

```
Template: "Diplomatic meeting between Iranian and {country} representatives, formal bilateral discussion, professional conference setting, {meeting_type}, balanced diplomatic photography, neutral perspective, 8K detail"

Variables:
Country: European Union, United Nations, neighboring countries
Meeting_type: trade negotiations, peace talks, cultural exchange
```

#### 13.2 Economic and Business Templates

**Market and Commerce:**

```
Template: "Iranian {market_type} showing {activity}, professional business photography, economic development theme, {atmosphere}, documentary business style, 8K detail"

Variables:
Market_type: stock exchange, bazaar, shopping district, industrial zone
Activity: trading activity, consumer shopping, industrial production
Atmosphere: bustling activity, steady growth, confident commerce
```

**Infrastructure and Development:**

```
Template: "Modern Iranian {infrastructure_type} demonstrating {development_aspect}, professional architectural photography, {lighting_time}, progress and modernization theme, 8K detail"

Variables:
Infrastructure_type: transportation hub, technology center, energy facility
Development_aspect: technological advancement, economic growth, sustainability
Lighting_time: golden hour, blue hour, bright daylight
```

#### 13.3 Cultural and Social Templates

**Cultural Events:**

```
Template: "Iranian {cultural_event} celebration, {participant_description}, traditional cultural photography, {atmosphere}, respectful cultural documentation, natural lighting, 8K detail"

Variables:
Cultural_event: Nowruz, poetry reading, art exhibition, music performance
Participant_description: diverse community gathering, family celebration, youth participation
Atmosphere: joyful celebration, solemn ceremony, artistic appreciation
```

**Educational and Academic:**

```
Template: "Iranian {educational_setting} with {participants}, academic atmosphere, {activity}, professional educational photography, inspirational learning environment, natural lighting, 8K detail"

Variables:
Educational_setting: university lecture hall, research laboratory, library, school classroom
Participants: students and professor, researchers, diverse learners
Activity: engaged learning, scientific research, academic discussion
```

### **Chapter 14: Troubleshooting and Problem-Solving**

#### 14.1 Common Technical Issues

**Poor Quality Outputs:**

**Problem**: Blurry, low-detail images **Solutions**:

1. Add quality boosters: "8K, UHD, sharp focus, professional photography"
2. Include camera specifications: "shot on professional DSLR"
3. Reduce CFG scale if too high (Stable Diffusion)
4. Use negative prompts: "blurry, low quality, amateur"

**Problem**: Anatomical deformities **Solutions**:

1. Comprehensive negative prompts for anatomy issues
2. Simplify poses and interactions
3. Use reference images when available
4. Generate multiple options and select best

**Problem**: Inconsistent style across images **Solutions**:

1. Use style reference images (--sref in Midjourney)
2. Maintain identical style descriptions
3. Lock seeds for similar compositions
4. Create detailed style templates

#### 14.2 Cultural and Content Challenges

**Problem**: Culturally inappropriate representations **Solutions**:

1. Include specific cultural context in prompts
2. Research appropriate dress codes and settings
3. Consult with cultural experts
4. Use positive examples as references

**Problem**: Stereotypical or biased outputs **Solutions**:

1. Be explicit about desired diversity
2. Use specific demographic descriptors
3. Include cultural authenticity keywords
4. Generate multiple options to avoid defaults

**Problem**: Achieving specific Iranian context **Solutions**:

1. Research and include accurate cultural details
2. Specify Persian architectural elements
3. Include appropriate clothing and settings
4. Use geographical and historical references

#### 14.3 Workflow Optimization

**Managing Tight Deadlines:**

**30-Minute Workflow:**

1. Use DALL-E 3 for speed and reliability
2. Employ pre-tested prompt templates
3. Accept first professional-quality result
4. Minimal post-processing

**2-Hour Workflow:**

1. Use Midjourney for better quality
2. Generate 3-4 options quickly
3. Quick client review and selection
4. Basic enhancement and formatting

**Same-Day Workflow:**

1. Use Stable Diffusion for maximum control
2. Multiple generation rounds with refinement
3. Comprehensive post-processing
4. Multiple format deliverables

**Client Communication Strategies:**

**Setting Expectations:**

- Explain AI capabilities and limitations
- Show example quality levels
- Discuss revision possibilities
- Clarify usage rights and restrictions

**Managing Revisions:**

- Use consistent prompting for modifications
- Leverage seed locking for variations
- Employ inpainting for specific changes
- Document successful prompt patterns

### **Chapter 15: Future-Proofing and Continuous Learning**

#### 15.1 Staying Current with AI Development

**Platform Updates and New Features:**

**Monitoring Strategy:**

- Follow official platform announcements
- Join professional AI communities
- Subscribe to industry newsletters
- Participate in beta testing programs

**Key Areas to Watch:**

- New parameter releases
- Model capability improvements
- Safety and ethical feature updates
- Integration tool developments

**Adapting to Changes:**

- Test new features with existing workflows
- Update template libraries regularly
- Retrain team on new capabilities
- Maintain backup workflows for transitions

#### 15.2 Building Professional Expertise

**Skill Development Pathway:**

**Foundation Level (Months 1-3):**

- Master basic prompt construction
- Learn platform-specific parameters
- Develop quality assessment skills
- Build template library

**Intermediate Level (Months 4-9):**

- Advanced consistency techniques
- Custom workflow development
- Integration with traditional tools
- Cultural adaptation mastery

**Advanced Level (Months 10+):**

- Custom model training (Stable Diffusion)
- Advanced batch production
- Team training and leadership
- Innovation and technique development

**Professional Community Engagement:**

- Join journalism and AI professional groups
- Share techniques and learn from peers
- Contribute to best practice development
- Stay informed on legal and ethical issues

**Continuous Improvement Process:**

1. **Weekly**: Review new techniques and tools
2. **Monthly**: Assess workflow efficiency
3. **Quarterly**: Update templates and standards
4. **Annually**: Comprehensive skill assessment and planning

---

## **APPENDICES**

### **Appendix A: Quick Reference Guides**

#### Essential Keyword Glossary

**Quality Boosters:**

- 8K, UHD, hyperdetailed, sharp focus, professional photography, award-winning, masterpiece, high resolution, ultra-realistic, photorealistic

**Lighting Terms:**

- Golden hour, blue hour, studio lighting, natural lighting, three-point lighting, Rembrandt lighting, butterfly lighting, soft light, hard light, dramatic lighting

**Camera Specifications:**

- 85mm lens, 50mm lens, macro lens, wide-angle, telephoto, shallow depth of field, deep depth of field, bokeh, shot on Canon, shot on Sony

**Composition Terms:**

- Rule of thirds, leading lines, symmetrical composition, wide shot, medium shot, close-up, low angle, high angle, eye level, overhead view

**Style Descriptors:**

- Documentary photography, editorial photography, professional portrait, journalistic style, news photography, commercial photography

#### Platform Parameter Quick Reference

**Midjourney:**

- `--ar 16:9` (widescreen), `--ar 1:1` (square), `--ar 9:16` (vertical)
- `--stylize 25` (realistic), `--stylize 100` (default), `--stylize 250` (artistic)
- `--chaos 10` (slight variation), `--chaos 25` (moderate), `--chaos 50` (high)
- `--quality 2` (high quality), `--quality 1` (standard)
- `--cref [URL]` (character reference), `--sref [URL]` (style reference)

**Stable Diffusion:**

- CFG Scale: 7-9 (recommended for journalism)
- Steps: 25-35 (balance of quality and speed)
- Sampler: DPM++ 2M Karras (reliable), Euler A (fast)
- Prompt weighting: `(keyword:1.3)` increase, `(keyword:0.8)` decrease

### **Appendix B: Cultural Sensitivity Checklist**

#### Pre-Generation Review

**Iranian Cultural Context:**

- [ ] Appropriate dress codes considered
- [ ] Religious sensitivities respected
- [ ] Traditional vs. modern balance appropriate
- [ ] Accurate cultural symbols and elements
- [ ] Respectful representation of authority figures

**International Representation:**

- [ ] Avoiding cultural stereotypes
- [ ] Neutral diplomatic presentation
- [ ] Balanced perspective maintained
- [ ] Respectful cross-cultural elements
- [ ] Appropriate formal protocols

#### Post-Generation Review

**Content Appropriateness:**

- [ ] No cultural misrepresentations
- [ ] Dignified portrayal of all subjects
- [ ] Accurate cultural details
- [ ] Professional journalistic standards
- [ ] Community sensitivity respected

### **Appendix C: Legal and Compliance Framework**

#### Copyright Considerations

**Safe Practices:**

- Substantial human modification of AI outputs
- Original concept development beyond AI generation
- Multiple source blending and transformation
- Documentation of creative process

**Risk Factors:**

- Direct commercial use without modification
- Replication of recognizable copyrighted styles
- Use of trademarked elements or logos
- Celebrity or public figure likeness issues

#### Iranian Media Compliance

**Professional Standards:**

- Respectful representation of government officials
- Appropriate cultural and religious sensitivity
- Balanced international coverage
- Factual accuracy in visual representation

**Technical Requirements:**

- Quality standards for broadcast and print
- Format specifications for different media
- Archive and documentation standards
- Distribution and usage guidelines

This comprehensive guide provides the foundation for professional text-to-image AI use in journalism, with specific attention to Iranian cultural context and international news coverage standards. Regular updates and community feedback will ensure continued relevance and effectiveness.
