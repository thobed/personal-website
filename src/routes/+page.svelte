<script>
    import Navbar from "./Navbar.svelte";
    import Tab1 from "./Tab1.svelte";
    import Tab2 from "./Tab2.svelte";
    import Tab3 from "./Tab3.svelte";
    import Tabs from "./Tabs.svelte";

    // List of tab items with labels, values and assigned components
    let items = [
        { label: "Content", value: 1, component: Tab1 },
        { label: "Interactions", value: 2, component: Tab2 },
        { label: "Tab 3", value: 3, component: Tab3 },
    ];
</script>

<link rel="preconnect" href="https://fonts.googleapis.com" />
<link rel="preconnect" href="https://fonts.gstatic.com" />
<link
    href="https://fonts.googleapis.com/css2?family=Roboto&display=swap"
    rel="stylesheet"
/>

<Navbar />
<div class="homepage_container">
    <div class="mainbody">
        <div class="whoami">
            <h1 class="myname">I'm Darrell Thobe.</h1>
            <h1>A Full Stack Software Engineer</h1>
        </div>

        <img class="homepageImage" src="darrell-thobe.png" />
    </div>
    <div class="mystatement">
        <p>
            I am a dependable and agile IT professional, known for architecting
            and developing innovative software solutions. My career is defined
            by a commitment to crafting custom software that meets complex
            challenges with creative and user-centric approaches. I believe that
            the most effective technological solutions emerge from a deep
            understanding of the end-users' needs. My expertise extends beyond
            technical proficiency in software development; it includes the
            ability to transform these skills into tangible, impactful results.
            With a strong work ethic and a passionate drive for technology, I
            excel in environments that value innovation and challenge
            conventional thinking. I am dedicated to continual learning and
            growth, always seeking to integrate cutting-edge technologies and
            methodologies into my practice. At the core of my professional ethos
            is the conviction that technology has the power to transform both
            lives and businesses. Whether through collaborative team dynamics or
            individual initiatives, my aim is to leave a lasting impact in the
            tech world by delivering solutions that are not only efficient and
            reliable but also accessible and intuitive to users.
        </p>
    </div>

    <div class="tabcontent">
        <Tabs {items} />
    </div>
    
</div>

