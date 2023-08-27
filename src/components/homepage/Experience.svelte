<script>
  import ExperienceCard from "./ExperienceCard.svelte"
</script>

<h5 class="underline mb-3">Experience</h5>
<ol>
  <li class="flex flex-col gap-y-4">
    <ExperienceCard
      project="JustProats"
      role="Software Developer"
      description="Built a fully customised Shopify Store from scratch, as the new site for the business. Will be available soon :)"
      link="https://justproats.com"
      badges={["Shopify", "Tailwind CSS", "TypeScript", "React.js"]}
      duration="Jul 2023 - Present"
      achievements={[
        "Designed a tailored custom theme to fit the company’s needs.",
        "Made a bundle subscription system using Recharge Payments API.",
        "Improved website speed by over 50 points.",
        "Focused on making the store customizable and automated through the Shopify CMS."
      ]}
    />
    <ExperienceCard
      project="Talking Cart"
      role="Software Developer"
      description={`Built key functionalities & UX of the chatbot. Engineered the backend to handle & optimize the "brain" logic.`}
      link="https://talkingcart.com"
      badges={["Next.js", "TypeScript", "OpenAI API", "Problem Solving"]}
      duration="Jun - Jul 2023"
      achievements={[
        "Used OpenAI API to recommend Amazon products based on input",
        "Developed an endpoint to get Amazon products based on keywords",
        "Made the logic to select a specific marketplace from 9 different regions according to user's location",
        "Designed an intuitive and user friendly interface"
      ]}
    />
  </li>
</ol>
