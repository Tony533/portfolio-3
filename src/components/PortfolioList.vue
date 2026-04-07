<script setup>
import PortfolioItem from './PortfolioItem.vue';

const projects = [
  {
    name: '(2025) LLM insights app for B2B behavioural data',
    description: 'This app combined enterprise visitor behavioural data, data bank of companies, addresses with media and financial disclosures available in the public domain to augment generated content offering insight to revenue builders, sales, marketers on how to best perform targeted outreach to potential and current customers.',
    technologies: ['Vue', 'TypeScript', 'NestJS', 'Vercel', 'Azure AI Foundry', 'Bedrock', 'GPT 5', 'OSS 120b', 'DynamoDB', 'AWS CDK', 'AWS SDK'],
    previewUrl: '',
    domain: '[n/a]',
    frontendSource: '',
    backendSource: '',
    imgUrls: []
  },
  {
    name: '(2025) Rapid prototyping tool for LLM generative content',
    description: 'This internal tool allowed for rapid prototyping of generative content solutions by providing a user-friendly interface to configure and test different prompt engineering techniques, LLMs and vector database configurations. It was used to quickly validate concepts and approaches for  use cases across the business.',
    technologies: ['TypeScript', 'Meow', 'Commander', 'Vercel', 'GPT 5', 'Claude', 'Gemini', 'AWS CDK'],
    previewUrl: '',
    domain: '[n/a]',
    frontendSource: '',
    backendSource: '',
    imgUrls: []
  },
  {
    name: '(2024) Value attribution and reporting platform',
    description: 'This platform was a key part of company\'s customer retention strategy. By collecting and using visitor data sources and using advanced attribution models with AB testing, it allowed customers to see changes in conversions and other high-value on-site behaviours. This insight underpinned customer\'s perception of earned value and the need to renew.',
    technologies: ['Vue', 'Apache ECharts', 'TypeScript', 'Express', 'NestJS', 'Redis', 'MSSQL', 'Snowflake', 'AWS CDK', 'AWS SDK'],
    previewUrl: '',
    domain: '[n/a]',
    frontendSource: '',
    backendSource: '',
    imgUrls: []
  },
  {
    name: '(2022) Search and locator platform for car buyers',
    description: 'An app allowing customers of a known luxury car manufacturer to \
      locate their desired vehicle for purchase.\
      Users can search, sort and filter new or used car stock by various vehicle attributes.\
      Different vehicles can be compared, favourited,\
      have their detailed specs viewed and used to generate hot leads through submitted enquiries.\
      The app is live on more than 100 sites in over 40 countries and supports some significant configurable feature\
      variation between them.',
    technologies: ['Vue', 'Vuetify', 'TypeScript', 'Express', 'GraphQL', 'Redis', 'AWS CDK', 'AWS SDK'],
    previewUrl: 'https://approved.es.landrover.com/search/#/',
    domain: 'landrover.com',
    frontendSource: '',
    backendSource: '',
    imgUrls: [
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture1.PNG',
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture2.PNG',
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture3.PNG',
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture4.PNG',
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture5.PNG',
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture6.PNG',
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture7.PNG',
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture8.PNG',
      'https://raw.githubusercontent.com/TonyPanczenko/TonyPanczenko.github.io/main/assets/ja/Capture9.PNG',
    ]
  },
  {
    name: '(2022) New enterprise user onboarding app',
    description: 'New enterprise users and customer accounts were launched using this internal portal. It allowed for product configuration management, automated communications, onboarding status management and contract management.',
    technologies: ['React', 'Python', 'Flask', 'SQLAlchemy', 'PostgreSQL'],
    previewUrl: '',
    domain: '[n/a]',
    frontendSource: '',
    backendSource: '',
    imgUrls: []
  },
  {
    name: '(2021) Stock locator for car configurator websites',
    description: 'This app allows users to find new vehicles which match their desired car\
    configuration in the best way possible. The backend service collects data from vehicle data libraries and stock\
    solutions to present the user with the closest approximate matches to maximise fullfilment. This solution serves\
    customers on dozens of North American and European model configurator sites.',
    technologies: ['React', 'Python', 'Flask', 'DynamoDB', 'AWS SDK', 'Serverless'],
    previewUrl: 'https://buildyour.jaguarusa.com/jag2/r/summary/inventory/en_us/\
e-pace_k23/49ojd/a-20p-249aawd_a-e-pace_sp2/',
    domain: 'buildyour.jaguarusa.com',
    frontendSource: '',
    backendSource: '',
    imgUrls: [
      '/assets/juc/Capture3.png',
      '/assets/juc/Capture1.png',
      '/assets/juc/Capture2.png',
      '/assets/juc/Capture4.png'
    ]
  },
  {
    name: '(2019) Crowd-sourced art project',
    description: 'This app lets any visitor paint a single pixel of a persistent image visible to anyone.\
    Users can see who and when painted each of the pixels. CDK proof of concept inspired by r/place.',
    technologies: ['React', 'Canvas', 'Node.js', 'NoSQL', 'AWS CDK', 'AWS SDK', 'CRA CLI', 'Webpack'],
    previewUrl: 'https://tony.panczenko.com/rplace-concept/',
    domain: 'tony.panczenko.com/rplace-concept',
    frontendSource: 'https://github.com/TonyPanczenko/rplace-concept',
    backendSource: 'https://github.com/TonyPanczenko/rplace-concept-backend',
    imgUrls: [
      '/assets/rplaceconcept/Capture1.png',
    ]
  },
  {
    name: '(2021) This portfolio app',
    description: 'This minimalistic portfolio page, you are looking at right now, was built using some of Vue\'s\
    newest features at the time and some of Quasar\'s fantastic carousel APIs. Thank you for browsing.',
    technologies: ['Vue', 'Quasar', 'Vite'],
    previewUrl: 'https://tony.panczenko.com/',
    domain: 'tony.panczenko.com',
    frontendSource: 'https://github.com/TonyPanczenko/portfolio-3',
    backendSource: '',
    imgUrls: [
      '/assets/portfolio/Capture1.png',
    ]
  },
];
</script>

<template>
	<div class="list">
		<PortfolioItem v-for="project in projects" :project="project" :key="project.name" />
	</div>
</template>

<style scoped lang="scss">

</style>
