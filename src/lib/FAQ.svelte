<script lang="ts">
  // FAQ component
  let openIndex: number | null = null;

  const faqs = [
    {
      question: "What is a prediction market?",
      answer: "A prediction market is a platform where people trade on the outcome of future events. The price of a share reflects the market's collective belief in the probability of that event occurring."
    },
    {
      question: "How does Polymarket ensure accuracy?",
      answer: "Polymarket uses 'skin in the game.' Because traders stand to profit or lose money based on the accuracy of their predictions, they are incentivized to seek out and trade on the best possible information, leading to highly accurate market odds."
    },
    {
      question: "How do I start trading?",
      answer: "Simply connect your crypto wallet (like MetaMask or Coinbase Wallet), deposit USDC, and you can start trading on any available market immediately. No traditional bank account required."
    },
    {
      question: "Is Polymarket decentralized?",
      answer: "Yes, Polymarket is built on the Polygon blockchain. All trades and settlements are handled by transparent smart contracts, ensuring that no single entity has control over your funds or the market outcomes."
    },
    {
      question: "How are markets settled?",
      answer: "Markets are settled based on verifiable real-world outcomes. We use decentralized oracles and clear resolution criteria defined for each market to ensure fair and transparent settlement."
    },
    {
      question: "What is the Polymarket leaderboard?",
      answer: "The leaderboard tracks the top traders on the platform by profit and loss. You can see the performance of top traders across different timeframes (24h, 7d, 30d, all-time) and even follow their wallets to see their latest trades."
    },
    {
      question: "How do I follow a trader?",
      answer: "You can click on any username or wallet address on the leaderboard or in the activity feed to view their profile. From there, you can follow them to get alerts on their trading activity."
    },
    {
      question: "What are the fees?",
      answer: "Polymarket is designed for high-frequency trading with minimal fees. Because it's on Polygon, gas fees are negligible, and the platform takes a small percentage of trading volume to maintain liquidity and operations."
    }
  ];

  function toggle(index: number) {
    openIndex = openIndex === index ? null : index;
  }
</script>

<section class="px-6 py-24 bg-white border-b border-gray-100">
  <div class="grid grid-cols-1 md:grid-cols-12 gap-8">
    <div class="md:col-span-4">
      <h2 class="text-3xl md:text-5xl font-bold text-gray-900 mb-6 max-w-xs leading-tight">
        Frequently asked questions
      </h2>
      <p class="text-gray-500 mb-8 max-w-xs">Everything you need to know about trading on the world's largest prediction market.</p>
      <a href="/" class="inline-flex items-center gap-2 text-sm font-bold text-primary-600 hover:gap-3 transition-all">
        Visit Help Center <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14M12 5l7 7-7 7"/></svg>
      </a>
    </div>
    <div class="md:col-span-8">
      <div class="border-t border-gray-100">
        {#each faqs as faq, i}
          <div class="border-b border-gray-100">
            <button 
              class="w-full py-8 flex items-center justify-between text-left hover:bg-gray-50 transition-colors group px-4 rounded-xl"
              onclick={() => toggle(i)}
            >
              <span class="text-lg font-semibold text-gray-900 group-hover:text-primary-600 transition-colors">{faq.question}</span>
              <span class="text-primary-500 font-light text-2xl ml-4">
                {openIndex === i ? '−' : '+'}
              </span>
            </button>
            {#if openIndex === i}
              <div class="pb-8 px-4 text-base text-gray-600 leading-relaxed max-w-2xl">
                {faq.answer}
              </div>
            {/if}
          </div>
        {/each}
      </div>
    </div>
  </div>
</section>
