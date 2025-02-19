<script>
  import { Title, ContactInfo, Card, CardSkillItem } from '$lib';
  
  const experience = [
        {
            title: "Full-Stack Developer",
            description: "2020-Pesent | Letsmove I.K.E"
        },
        {
            title: "Full-Stack Developer",
            description: "2019-Pesent | Tatitech Llc."
        },
        {
            title: "Full-Stack Developer",
            description: "2018-2019 | Iek Akmi"
        },
        {
            title: "Full-Stack Developer",
            description: "2018-2019 | Metropolitan College"
        },
        {
            title: "Full-Stack Developer",
            description: "2016-2018 | Webplanners"
        },
        {
            title: "SEO Specialist - Part Time",
            description: "2017 | Energy24"
        },    
        {
            title: "Full-Stack Developer",
            description: "Contract | Netwise I.K.E"
        }
    ]

  const education = [
    {
      subtitle: "2015-2017 | Greece",
      title: "Web Development & Game Design",
      description: "IEK AKMI"
    },
    {
      subtitle: "2019-2022 | Greece",
      title: "Computer & Network Technician",
      description: "Technical / Vocational Education"
    }
  ]

  const certification = [
    {
      title: "ScrumMaster",
      description: "Scrum Alliance"
    },
    {
      title: "Pre Security",
      description: "TryHackMe"
    },
    {
      title: "AI Agents Fundamentals",
      description: "Hugging Face"
    },
    {
      title: "Deep Dive on Container Security",
      description: "Amazon AWS"
    },
    {
      title: "Containers",
      description: "Amazon AWS"
    },
    {
      title: "Fragate Introduction",
      description: "Amazon AWS"
    }
  ]

  const skills = [
    { title: "JavaScript" },
    { title: "Node.js" },
    { title: "Svelte" },
    { title: "Vue" },
    { title: "PHP" },
    { title: "HTML5 & CSS3" },
    { title: "jQuery" },
    { title: "SVG's" },
    { title: "Tailwind CSS" },
    { title: "React" },
    { title: "NoSQL" },
    { title: "MySQL" },
    { title: "Linux" },
    { title: "Git" },
    { title: "API's" },
    { title: "Laravel" },
    { title: "Wordpress" },
    { title: "Prestashop" },
    { title: "Joomla" },
    { title: "Adobe Suite" },
    { title: "SEO" },
    { title: "Cpanel" },
    { title: "Plesk" },
    { title: "WHM" },
    { title: "Servers" },
    { title: "Analytics" },
    { title: "Tagging" }
  ]

  const tools = [
    { link: "/assets/img/javascript.png" },
    { link: "/assets/img/svelte.png" },
    { link: "/assets/img/tailwind.png" },
    { link: "/assets/img/wordpress.png" },
    { link: "/assets/img/vscode.png" },
    { link: "/assets/img/php.png" },
    { link: "/assets/img/mysql.png" },
  ]
</script>

<!-- Flex Row -->
<div class="pt-10 pb-10 md:flex md:flex-row md:space-x-8">
  <!-- Column 1 -->
  <div class="flex flex-col flex-2 text-white">
    <Title />
    <ContactInfo />
    <Card 
      data={experience}
      title="Experience" 
      bgTitle="#f1619c" 
      animationClasses="animate__animated animate__backInLeft animate_fast"
    />
  </div>
  <!-- End Column 1 -->

  <!-- Column 2 -->
  <div class="flex flex-col flex-2 text-white">
    <Card 
      data={education}
      title="Education" 
      bgTitle="#b1e82e"
      titleColor="#090516" 
      rotateTitle="rotate-3"
      animationClasses="animate__animated animate__backInDown animate__slow"
    />

    <Card 
      data={certification}
      title="Certifications" 
      bgTitle="#6b57ff"
      animationClasses="animate__animated animate__backInUp animate__slow"
    />
  </div>
  <!-- End Column 2 -->

  <!-- Column 3 -->
  <div class="flex flex-col flex-2 text-white">
    <Card 
      data={skills}
      type="single"
      title="Skills" 
      bgTitle="#f5dbdb" 
      titleColor="#090516"
      animationClasses="animate__animated animate__backInRight animate__fast"
    />
    
    <Card 
      data={tools}
      type="image"
      title="Favorite Tools" 
      bgTitle="#f1619c"
      rotateTitle="rotate-3"
      animationClasses="animate__animated animate__backInRight animate__slow"
    />

    <Card 
      data={null}
      type="static"
      title="About me" 
      bgTitle="#b1e82e"
      titleColor="#090516" 
      animationClasses="animate__animated animate__backInRight animate__fast"
    />
  </div>
  <!-- End Column 3 -->
</div>         
<!-- End Flex Row -->
