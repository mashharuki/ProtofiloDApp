<script>
    let projects = [
        { name: 'ETH dApp', url: 'https://my-wave-portal-flame.vercel.app/' },
        { name: 'ETH NFT Collection', url: 'https://my-wave-portal-flame.vercel.app/' },
        { name: 'Generative NFT', url: 'https://generative-nftda-pp.vercel.app/'},
        { name: 'SolanaDApp', url: 'https://solana-da-pp.vercel.app/' },
        { name: 'SolanaNFTDApp', url: 'https://solana-nftd-rop-app.vercel.app/' },
        { name: 'Web3MedicalDApp', url: 'https://web3-medical-dapp.vercel.app/DoctorInfo' },
        { name: 'SolanaWalletDApp', url: 'https://solana-wallet-da-pp.vercel.app/' },
        { name: 'MyENSDApp', url: 'https://myensdapp.vercel.app/' },
        { name: 'SolanaOnlineStore', url: 'https://myensdapp.vercel.app/' },
        { name: 'MultiSigWalletDApp', url: 'https://multi-sig-wallet-contract.vercel.app/' },
        { name: 'NearHotelBooking', url: 'https://naer-hotel-booking-dapp.netlify.app/' },
        { name: 'NearElectionDApp', url: 'https://nearelectiondapp.netlify.app/' },
        { name: 'ETH NFT Maker', url: 'https://my-nftm-aker-oiry51z6c-mashharuki.vercel.app/' },
        { name: 'ETH NFT Game', url: 'https://my-nftg-ame.vercel.app/' },
    ];
</script>

<section id="portfolio">
    <div class="container mx-auto">
        <div class="py-32">
            <h1 class="text-center mb-10 font-medium text-3xl">PORTFOLIO</h1>
            <div class="flex flex-wrap lg:w-4/5 sm:mx-auto">
                <!-- roop -->
                {#each projects as project}
                <div class="p-2 md:w-1/3 w-full">
                    <div class="
                        bg-gray-400 
                        text-white 
                        hover:bg-gray-800 
                        cursor-pointer 
                        rounded p-4 
                        text-center "
                    >
                        <a href={project.url}>{project.name}</a>
                    </div>
                </div>
                {/each}
            </div>
        </div>
    </div>
</section>