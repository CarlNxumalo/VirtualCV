<script>
  import { Section, News, HeroHeader, HeroBody, ContentWithImage,Cta } from 'flowbite-svelte-blocks';
  import { ArrowRightOutline, VideoCameraSolid } from 'flowbite-svelte-icons';
  import { Button } from 'flowbite-svelte';
  import { Li, List, P} from 'flowbite-svelte';
  import {  Contact } from 'flowbite-svelte-blocks';
  import { Label, Input, Textarea } from 'flowbite-svelte';
  import {  FeatureDefault, FeatureItem } from 'flowbite-svelte-blocks';
  import { ChartPieSolid, LandmarkSolid, BriefcaseSolid, DollarOutline, RocketSolid, CogOutline } from 'flowbite-svelte-icons';
  import { Footer, FooterBrand, FooterLinkGroup, FooterLink, FooterCopyright, FooterIcon } from 'flowbite-svelte';
</script>

<Section name="heroDefault">
  <HeroHeader>
    <svelte:fragment slot="h1">Carl Nxumalo, The Fullstack Software Developer And Data Analyst</svelte:fragment>
    
    <svelte:fragment slot="paragraph">I am a motivated individual passionate about software
        development and eager to make a positive impact on
        South Africa's IT industry. I am committed to enhancing
        my skills and acquiring the knowledge needed to become
        a proficient software developer</svelte:fragment>
    
  </HeroHeader>
  <div class="flex flex-col mb-8 lg:mb-16 space-y-4 sm:flex-row sm:justify-center sm:space-y-0 sm:space-x-4">
    <a href="/">
      <Button size="lg" color="red">
        Contact Me <ArrowRightOutline size="md" class="ml-2 -mr-1" />
      </Button>
    </a>
    
  </div>
  
</Section>
<div id="MySkills"></div>
<Section name="feature" id="MySkills">
  <HeroHeader class="max-w-screen-md mb-8 lg:mb-16" h2Class="mb-4 text-4xl tracking-tight font-extrabold text-gray-900 dark:text-white" pClass="text-gray-500 sm:text-xl dark:text-gray-400">
    <svelte:fragment slot="h2">My Skill Set</svelte:fragment>
    <svelte:fragment slot="paragraph">
      My skill set centers on data management and data analytics, including descriptive analytics and a touch of machine learning. I specialize in creating information systems that streamline business functions, enabling organizations to make data-driven decisions and operate more efficiently.
    </svelte:fragment>
  </HeroHeader>
  <FeatureDefault>
    <FeatureItem>
      <svelte:fragment slot="icon"><ChartPieSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Database Design</svelte:fragment>
      <svelte:fragment slot="paragraph">I have extensive experience in designing efficient and scalable databases for various applications. My expertise includes utilizing relational databases to ensure robust data management.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><LandmarkSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Object Orieantated Programming</svelte:fragment>
      <svelte:fragment slot="paragraph">I create modular and maintainable code, ensuring complex systems are broken down into reusable and scalable components.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><BriefcaseSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Cloud</svelte:fragment>
      
      <svelte:fragment slot="paragraph">I utilize cloud platforms such as Vercel, Azure, and Supabase to deploy and manage applications efficiently. My experience includes leveraging these services for scalable hosting, database management, and seamless integration.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><DollarOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Data Analystics</svelte:fragment>
      <svelte:fragment slot="paragraph">I transform your data into easy-to-understand insights, enabling better business decisions. My expertise includes using advanced analytics techniques to interpret complex data and provide actionable recommendations.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><RocketSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Web & Desktop development</svelte:fragment>
      <svelte:fragment slot="paragraph">Craft beautiful, delightful experiences for both marketing and product with real cross-company collaboration.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><CogOutline class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Machine Learning & AI</svelte:fragment>
      <svelte:fragment slot="paragraph">I have utilized open-source machine learning models in real-world applications. Using tools from Hugging Face and Python libraries like scikit-learn</svelte:fragment>
    </FeatureItem>
  </FeatureDefault>
</Section>
<div id="MyStack"></div>
<Section name="ctawithimg" id="MyStack">
  <Cta ctatype="image">
    <svelte:fragment slot="img">
      <img class="w-full dark:hidden" src="/LightModeStack.png" alt="dashboard" />
      <img class="w-full hidden dark:block" src="/LightModeStack.png" alt="dashboard" />
    </svelte:fragment>
    <svelte:fragment slot="h2">Modern Technologies</svelte:fragment>
    <List tag="ul" class="space-y-1 text-gray-500 dark:text-gray-400">
      <Li>Supabase: an open source Firebase alternative.</Li>
      <Li>Vercel: provides the developer tools and cloud infrastructure </Li>
      <Li>Azure: One of the biggest and most trusted cloud provider</Li>
      <Li>Databases: Microsoft SQL
        Server, PostgreSQL,
        Oracle
      </Li>
      <Li>Frameworks: SvelteKit,
        Node.js, .NET Framework
      </Li>
      <Li>Languages: C#, Java,
        Python, Java Script
        HTML & CSS</Li>
      
    </List>
  </Cta>
</Section>
<div id="MyProjects"></div>
<Section name="ctawithimg" id="MyProjects">
    <Cta ctatype="image">
      <svelte:fragment slot="img">
        <img class="w-full dark:hidden" src="/minbox2.png" alt="dashboard" />
        <img class="w-full hidden dark:block" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/cta/cta-dashboard-mockup-dark.svg" alt="dashboard" />
      </svelte:fragment>
      <svelte:fragment slot="h2">Latest Project MIN-BOX, a web-based academic communication tool</svelte:fragment>
      <p class="mb-6 font-light text-gray-500 md:text-lg dark:text-gray-400">
        Developed a SvelteKit application to address
        repeated student messages sent to lecturers.
        Created a public mailbox system where students
        can view messages sent to lecturers, reducing
        duplicate inquiries.
        Integrated NLP search functionality (using
        sentence-transformers/paraphrase-multilingualMiniLM-L12-v2 API) to find and display similar
        messages.
        Improved communication efficiency between
        students and lecturers by minimizing message
        redundancy.

      </p>
      <a href="https://minbox-vert.vercel.app/" class="inline-flex items-center text-white bg-primary-700 hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:focus:ring-primary-900">
        View Project
        <ArrowRightOutline size="md" class="ml-2 -mr-1" />
      </a>
    </Cta>
</Section>

  <Section name="ctawithimg">
    <Cta ctatype="image">
      <svelte:fragment slot="img">
        <img class="w-full dark:hidden" src="/FNBChallenge.png" alt="dashboard" />
        <img class="w-full hidden dark:block" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/cta/cta-dashboard-mockup-dark.svg" alt="dashboard" />
      </svelte:fragment>
      <svelte:fragment slot="h2">FNB Data Quest Challenge</svelte:fragment>
      <p class="mb-6 font-light text-gray-500 md:text-lg dark:text-gray-400">
        Analyzed customer data to predict loan repayment
        likelihood using logistic regression.
        Built a predictive model to assess loan repayment
        probabilities, aiding in risk management.
        Applied statistical methods to clean and preprocess
        large datasets, ensuring data accuracy and
        reliability.
        Provided actionable insights into customer behavior
        and repayment trends, supporting informed
        decision-making with 95% accuracy.        
      </p>
      <a href="https://deepnote.com/workspace/test-bb06-62867fec-ec2b-48aa-b4ab-911e1572fe9d/project/FNB-Data-Quest-Carl-Nxumalo-f45e2069-056a-4192-9936-7b59ee37bd3e/notebook/Scoring-27dd4516580842398f92475f47508362" class="inline-flex items-center text-white bg-primary-700 hover:bg-primary-800 focus:ring-4 focus:ring-primary-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center dark:focus:ring-primary-900">
        View Project
        <ArrowRightOutline size="md" class="ml-2 -mr-1" />
      </a>
    </Cta>
  </Section>

  <div id="MyEducation"></div>
<Section name="cta" id="MyEducation">
    <Cta>
        <svelte:fragment slot="h2">My Education</svelte:fragment>
        <P size="xl">Bachelor of Science in Information Technology
        </P>
        <p class="mb-6 font-light text-gray-500 dark:text-gray-400 md:text-lg">
            I am a final-year student at North-West University, set to graduate in 2024 with a Bachelor of Science in Information Technology. Throughout my studies, I have earned 25 distinctions out of 26 modules and maintained an academic average of 83%. I am also a proud SAP bursary student.
        </p>
        <P size="xl">Matriculated At Beaulieu College 
        </P>
        <p class="mb-6 font-light text-gray-500 dark:text-gray-400 md:text-lg">
            I attended Beaulieu College from 2016 to 2020, where I was recognized as the best rugby player and the most academically improved student. My time there was filled with growth, both on the field and in the classroom.
        </p>
    </Cta>
</Section>

<div id="MyAbout"></div>
<Section name="contentwithimg">
  <ContentWithImage>
      <svelte:fragment slot="h2">About Me</svelte:fragment>
      <p class="mb-4">
          Born in Johannesburg in 2002, I have always cherished the moments spent with friends and family, valuing the bonds that bring joy and meaning to life. Alongside my social nature, I have a deep passion for programming, finding immense satisfaction in solving complex problems and creating innovative solutions. Here are a few key points about me:
      </p>
      <List tag="ul" class="space-y-1 text-gray-500 dark:text-gray-400">
          <Li>Background: Johannesburg native with a rich cultural heritage.</Li>
          <Li>Social: Enjoys spending quality time with friends and family.</Li>
          <Li>Technical: Enthusiastic about programming and technology.</Li>
          <Li>Goals: Aim to combine social skills and technical expertise to contribute meaningfully to the tech community.</Li>
      </List>

      <svelte:fragment slot="image">
      <img class="w-full rounded-lg" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/content/office-long-2.png" alt="office content 1" />
      <img class="mt-4 w-full lg:mt-10 rounded-lg" src="https://flowbite.s3.amazonaws.com/blocks/marketing-ui/content/office-long-1.png" alt="office content 2" />
      </svelte:fragment>
  </ContentWithImage>
</Section>

<div id="MyContact"></div>
  <Section name="contact" id="MyContact">
    <Contact>
      <svelte:fragment slot="h2">Contact Me</svelte:fragment>
      <svelte:fragment slot="paragraph">Got a technical issue? Want to send feedback about a beta feature? Need details about our Business plan? Let us know.</svelte:fragment>
      <form class="space-y-8">
        <div>
          <Label for="email" class="block mb-2">Your email</Label>
          <Input id="email" name="email" placeholder="carl.bongani@gmail.com" required />
        </div>
        <div>
          <Label for="subject" class="block mb-2">Subject</Label>
          <Input id="subject" name="subject" placeholder="Subject" required />
        </div>
        <div>
          <Textarea id="subject" name="subject" placeholder="Leave a comment..." label="Your message" />
        </div>
        <Button>Send message</Button>
      </form>
    </Contact>
  </Section>


  
  <Footer footerType="socialmedia">
    <div class="mx-auto max-w-screen-xl text-center">
      <FooterBrand href="https://flowbite.com" src="/images/logo.svg" alt="Flowbite Logo" name="Flowbite" aClass="flex justify-center items-center text-2xl font-semibold text-gray-900 dark:text-white" />
      <p class="my-6 text-gray-500 dark:text-gray-400">Open-source library of over 400+ web components and interactive elements built for better web.</p>
      <FooterLinkGroup ulClass="flex flex-wrap justify-center items-center mb-6 text-gray-900 dark:text-white">
        <FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="https://github.com/CarlNxumalo">Github</FooterLink>
        <FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="https://www.linkedin.com/in/carl-nxumalo-bb34a1282/">LinkedIn</FooterLink>
      </FooterLinkGroup>
      <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400">2024</span>
    </div>
  </Footer>