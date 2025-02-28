<script>
  import { Section, News, HeroHeader, HeroBody, ContentWithImage,Cta } from 'flowbite-svelte-blocks';
  import { ArrowRightOutline, DatabaseSolid, CodeBranchSolid, CloudArrowUpSolid,ComputerSpeakerSolid, BrainSolid } from 'flowbite-svelte-icons';
  import { Button } from 'flowbite-svelte';
  import { Li, List, P, Heading} from 'flowbite-svelte';
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
    <a href="/Carl Nxumalo CV.pdf">
      <Button size="lg" color="red">
        Download My CV <ArrowRightOutline size="md" class="ml-2 -mr-1" />
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
      <svelte:fragment slot="icon"><DatabaseSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Database Design</svelte:fragment>
      <svelte:fragment slot="paragraph">I have extensive experience in designing efficient and scalable databases for various applications. My expertise includes utilizing relational databases to ensure robust data management.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><CodeBranchSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Object-Oriented Programming</svelte:fragment>
      <svelte:fragment slot="paragraph">I create modular and maintainable code, ensuring complex systems are broken down into reusable and scalable components.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><CloudArrowUpSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Cloud</svelte:fragment>
      
      <svelte:fragment slot="paragraph">I utilize cloud platforms such as Vercel, Azure, and Supabase to deploy and manage applications efficiently. My experience includes leveraging these services for scalable hosting, database management, and seamless integration.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><ChartPieSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Data Analystics</svelte:fragment>
      <svelte:fragment slot="paragraph">I transform your data into easy-to-understand insights, enabling better business decisions. My expertise includes using advanced analytics techniques to interpret complex data and provide actionable recommendations.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><ComputerSpeakerSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
      <svelte:fragment slot="h3">Web & Desktop development</svelte:fragment>
      <svelte:fragment slot="paragraph">I develop user-centric web and desktop applications that are visually appealing and functionally robust, ensuring seamless experiences across platforms with modern frameworks and technologies.</svelte:fragment>
    </FeatureItem>
    <FeatureItem>
      <svelte:fragment slot="icon"><BrainSolid class="text-primary-600 dark:text-primary-300" /></svelte:fragment>
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
  </ContentWithImage>
</Section>

<div id="MyContact"></div>
  
<Footer footerType="socialmedia">
  <div class="mx-auto max-w-screen-xl text-center">
    <Heading tag="h2" customSize="text-4xl font-extrabold ">Contact Me</Heading>
    <p class="my-6 text-gray-500 dark:text-gray-400">"Don’t hesitate to reach out to me through any of the platforms available. I’m always here to help!"</p>
    <FooterLinkGroup ulClass="flex flex-wrap justify-center items-center mb-6 text-gray-900 dark:text-white">
      <FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="https://github.com/CarlNxumalo">Github</FooterLink>
      <FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="https://www.linkedin.com/in/carl-nxumalo-bb34a1282/">LinkedIn</FooterLink>
      <FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="mailto:carl.ybongani@gmail.com">carl.ybongani@gmail.com</FooterLink>
      <FooterLink liClass="" aClass="mr-4 hover:underline md:mr-6" href="tel:+27716367633">071 636 7633</FooterLink>
    </FooterLinkGroup>
    <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400">2024/08/02</span>
  </div>
</Footer>