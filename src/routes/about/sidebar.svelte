<script lang="ts">
    import { Button } from "$lib/components/ui/button";
    import { Card } from "$lib/components/ui/card";
    
    const sidebarItems = [
      'About Overview',
      'Our Mission',
      'Management',
      'Our History',
      'Frequently Asked Questions',
      'Awards & Accolades',
      'International Linkages'
    ];
    
    const caseStudies = [
      "Ericsson's Proactive Supply Chain Risk Management",
      "Yesware's Matthew Bellows on His Ironic Challenge",
      "Maclaren's Stroller Recall: What Would You Do?"
    ];
    </script>
    
    <div class="w-full md:w-3/5">
      <Card class="p-6 mb-8">
        <h2 class="text-2xl font-bold mb-4">About Us</h2>
        <ul class="space-y-2">
          {#each sidebarItems as item}
            <li class="hover:bg-gray-100 p-2 rounded">{item}</li>
          {/each}
        </ul>
      </Card>
    </div>