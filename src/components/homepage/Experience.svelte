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
    />
    <ExperienceCard
      project="Talking Cart"
      role="Software Developer"
      description={`Built key functionalities & UX of the chatbot. Engineered the backend to handle & optimize the "brain" logic.`}
      link="https://talkingcart.com"
      badges={["Next.js", "TypeScript", "OpenAI API", "Problem Solving"]}
      duration="Jun - Jul 2023"
    />
  </li>
</ol>
