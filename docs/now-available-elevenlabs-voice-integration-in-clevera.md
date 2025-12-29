---
title: "Now Available: ElevenLabs Voice Integration in Clevera"
created_at: "2025-12-19T14:27:15+03:00"
updated_at: "2025-12-19T14:30:17+03:00"
source: "Clevera"
---

> 📺 **Watch the video tutorial**: [https://share.clevera.ai/embed/?id=video_dstbmg8xhl50nehz&token=oO0jXdhdtECAwRddu7tfd7F13JJNLxlm&type=video-only](https://share.clevera.ai/embed/?id=video_dstbmg8xhl50nehz&token=oO0jXdhdtECAwRddu7tfd7F13JJNLxlm&type=video-only)


> high_voltage **TL;DR:** To integrate ElevenLabs, generate an API key in ElevenLabs with Text-to-Speech (Access), Voices (Read), Models (Read), and User (Read) permissions, then paste and save this key in Clevera's Account Settings before regenerating a video with ElevenLabs as the voice engine.

Elevate Your Videos with ElevenLabs Voices in Clevera

Creating compelling product videos often requires a distinctive voice that resonates with your brand and audience. While Clevera offers a range of voice options, integrating advanced AI voice generation platforms like ElevenLabs allows for unparalleled customization and high-quality synthetic voices. This tutorial will guide you through the seamless process of connecting your ElevenLabs account with Clevera, enabling you to regenerate your video voiceovers with custom, professional voices that truly stand out.

By the end of this guide, you will have successfully generated an ElevenLabs API key with the precise permissions required for Clevera, linked your ElevenLabs account to Clevera, and regenerated a video using an ElevenLabs voice. This integration unlocks a new level of audio fidelity and personalization for your video content within the Clevera platform.

To follow along, you'll need an active ElevenLabs account and a Clevera workspace where you can manage your video projects. Please ensure you have administrator access to both platforms to modify API keys and account settings.

---

## Generating Your ElevenLabs API Key

To connect ElevenLabs with Clevera, you first need to generate a specific API key within your ElevenLabs account. This key acts as a secure credential, allowing Clevera to access ElevenLabs' voice generation capabilities on your behalf. It's crucial to set the correct permissions for this key to ensure full functionality within Clevera while maintaining security.

### Step 1: Navigate to the ElevenLabs Developers Page

Begin by logging into your ElevenLabs account. Once logged in, you'll land on your creative platform dashboard, which displays various content creation options and your workspace summary.

In the left-hand navigation sidebar, locate and click on the **Developers** option. This section provides access to API keys, webhooks, usage data, and documentation for integrating ElevenLabs with other applications.

### Step 2: Access the API Keys Panel

After navigating to the **Developers** page, you'll see several tabs at the top: **Overview**, **API Keys**, **Webhooks**, and **Usage**.

Click on the **API Keys** tab. This panel lists any existing API keys associated with your account and provides options to manage them. You can create multiple keys, each with different access levels, for various integrations.

### Step 3: Create a New API Key

On the **API Keys** panel, locate the **+ Create Key** button on the right side of the "User API Keys" section.

Click this **+ Create Key** button. A "Create API Key" sidebar will slide open from the right, presenting various configuration options for your new key.

### Step 4: Configure API Key Permissions for Clevera

The "Create API Key" sidebar allows you to define the name and permissions for your new API key.

#### Name Your API Key

At the top of the sidebar, in the **Name** field, enter a descriptive name for your API key, such as _Clevera Integration_ or _Clevera Voiceovers_. This helps you identify the key's purpose later.

#### Set Endpoints and Access Levels

Scroll down to the **Endpoints** section. Here, you'll see a list of ElevenLabs features, each with its own access settings. For Clevera to function correctly, specific permissions must be granted:

1. **Text-to-Speech:** This is the primary service Clevera will use to generate voiceovers.Find the **Text-to-Speech** row.  Click the **Access** button next to it. It will change from "No Access" to "Access," indicating that this endpoint is enabled.
2. **Voices:** Clevera needs to be able to read available voices from your ElevenLabs account to allow you to select them.Scroll down to find the **Voices** row under the "Voice Generation" section.  Click the **Read** button. It will change from "No Access" to "Read."  _Other visible options for Voices:_ You'll also see a **Write** button. Granting "Write" access for Voices would allow external applications to create or modify voices in your ElevenLabs account. For Clevera's voiceover regeneration, only "Read" access is necessary.
3. **Models:** Clevera needs to read the available voice models.Scroll down further to find the **Models** row under the "Administration" section.  Click the **Read** button. It will change from "No Access" to "Read."  _Other visible options for Models:_ Similar to Voices, a **Write** button is present. "Write" access for Models would enable creating or modifying voice models, which is not required for Clevera.
4. **User:** Clevera needs to read basic user information to verify the API key and ensure it's valid.Locate the **User** row, also under the "Administration" section.  Click the **Read** button. It will change from "No Access" to "Read."  _Other visible options for User:_ The **Write** button would allow modification of user data, which is not needed for this integration.

> [!TIP]
> **Best Practice:** Only grant the minimum necessary permissions to API keys. This "least privilege" principle enhances security by limiting potential damage if a key is compromised. For Clevera, the `Text-to-Speech: Access`, `Voices: Read`, `Models: Read`, and `User: Read` permissions are sufficient.

#### Review Other Endpoints

As you configure the permissions, briefly review other endpoints to ensure they remain at "No Access" or default "No Read/Write" unless you have specific needs beyond Clevera integration.

For example, `Speech to Speech`, `Speech to Text`, `Sound Effects`, `Audio Isolation`, `Dubbing`, `ElevenLabs Agents`, `Projects`, `Audio Native`, `Voice Generation`, `Forced Alignment`, `Music Generation`, `History`, `Pronunciation Dictionaries`, and `Workspace` all default to "No Access" or "No Read/Write," which is appropriate for this integration.

### Step 5: Finalize and Copy Your API Key

Once you have configured the permissions as described above, click the **Create Key** button at the bottom right of the sidebar.

A modal window will appear, titled "API Key – [Your Key Name]," displaying your newly generated API Key. This is the **only time** the full key will be shown for security reasons.

Click the **Copy to Clipboard** button within this modal. A small notification will confirm "API key copied to clipboard."

> [!WARNING]
> **Important:** Do not close this modal until you have successfully copied the API key. Once closed, you will not be able to retrieve the full key again. If you lose it, you'll need to generate a new one.

You can now click **Close** on the modal. Your ElevenLabs API key is now ready for use in Clevera.

---

## Connecting ElevenLabs to Clevera and Regenerating Voiceovers

With your ElevenLabs API key safely copied, the next step is to integrate it into your Clevera workspace and leverage it to create engaging voiceovers for your videos. This involves updating your Clevera account settings and then selecting ElevenLabs as your preferred voice engine when regenerating a video.

> [!TIP]
> Make sure you have administrator access to both ElevenLabs and Clevera before starting — you'll need it to create API keys and update workspace settings.

### Step 1: Navigate to Clevera Account Settings

Switch to your Clevera dashboard. In the top-left corner of the Clevera interface, you'll see your workspace name, typically accompanied by a dropdown arrow (e.g., **Antbees**).

Click on your workspace name. A dropdown menu will appear, displaying options such as **Account Settings**, **Team Settings**, **Usage**, **Billing**, and **Integrations**.

Click **Account Settings** from the dropdown menu. This will take you to your personal account configuration page.

### Step 2: Manage the ElevenLabs API Key in Clevera

On the **Account Settings** page, scroll down until you find the section titled "ElevenLabs API Key." This section is specifically designed for configuring your ElevenLabs integration.

If you have a previously entered (and potentially invalid) API key, you might see an obscured key (e.g., `sk_************dff09`) and an associated error message indicating issues with permissions (e.g., "Unable to access user information. Please check that your API key has 'User: Read' permission.").

To ensure a clean setup with your new, correctly configured API key:

1. **Clear the Existing Key:** Click the **Clear Key** button, located below the API key input field. This removes any old or incorrect API key data.A "API key removed successfully" notification will briefly appear at the bottom of the screen.
2. **Paste the New Key:** In the now empty **API Key** input field, right-click and select **Paste** from the context menu, or use your keyboard shortcut (Cmd+V on Mac, Ctrl+V on Windows) to paste the ElevenLabs API key you copied earlier. The field will populate with your new key.
3. **Save the New Key:** Click the **Save Key** button.

Clevera will then verify the API key's permissions. If successful, a "Verified" badge will appear next to "ElevenLabs API Key," and any previous error messages will disappear. This confirms that your Clevera workspace is now correctly connected to your ElevenLabs account.

> [!TIP]
> If the API key verifies successfully, Clevera will show a "Verified" status and remove permission-related errors — this indicates the integration is ready to use.

### Step 3: Navigate to Your Videos

After successfully linking your ElevenLabs account, you can now proceed to regenerate a video using these new voice options.

In the left-hand navigation sidebar, click on **My Videos**. This will take you back to your video library, displaying all your created and in-progress video projects.

### Step 4: Open a Video for Editing

From your **My Videos** list, select a video you wish to regenerate with an ElevenLabs voice.

Click on the video thumbnail or title to open it in the Clevera video editor. The video editor will load, showing your video content and timeline.

### Step 5: Initiate Voiceover Regeneration

Within the video editor, locate the **Revise** button in the top-right corner of the screen.

Click the **Revise** button. A dropdown menu will appear with options such as **Improve Voiceovers**, **Change Voice**, **Translate to...**, and **Regenerate Voiceovers**.

Click **Regenerate Voiceovers**. This action opens the "Regenerate Video" modal window, where you can configure various aspects of your video's new voiceover.

### Step 6: Select ElevenLabs as the Voice Engine

The "Regenerate Video" modal presents several options for customizing your video regeneration.

#### Review Generation Options

Briefly review the available regeneration options:

- **Type:** Choose the type of video generation, such as **How-to Guide**, **Onboarding**, **Product demo (tour)**, or **Feature Announcement**. The default selection is **How-to Guide**. These options influence the narrative style of the regenerated voiceover.
- **Language:** Select the language for your voiceover. The default is **English (US)**.
- **Tone:** Choose the desired tone for the voiceover, with options like **Casual**, **Formal**, **Motivational**, and **Persuasive**.
- **Voiceover Detail:** Control the level of detail in the voiceover narration, with options like **Minimal**, **Standard**, and **Detailed**.

#### Choose ElevenLabs

Scroll down to the **Voice Engine** section. Here, you'll see a selection of available voice providers: **Google**, **OpenAI**, and **ElevenLabs**.

Click on **ElevenLabs**. A tooltip might briefly appear, reminding you that "You will need to have an ElevenLabs subscription to use this provider." This confirms that Clevera recognizes your ElevenLabs integration.

> [!NOTE]
> Clevera supports multiple voice engines, allowing you to choose the best fit for your project. ElevenLabs is often chosen for its high-quality, natural-sounding, and customizable AI voices.

### Step 7: Select an ElevenLabs Voice

Once ElevenLabs is selected as the **Voice Engine**, a new dropdown menu labeled **Voice** will appear below it, showing the currently selected voice (e.g., "Sulatfat").

Click the **Voice** dropdown menu. A comprehensive list of available ElevenLabs voices will populate, categorized by "All," "Male," and "Female." Each voice option displays its name (e.g., "Roozbeh," "Adam," "Alice") and a brief description (e.g., "Male | American," "Female | British").

Scroll through the list and select your desired voice. For this tutorial, the video demonstrates selecting **Roozbeh**. Click on the name of the voice you wish to use.

The dropdown menu will close, and the selected voice (e.g., "Roozbeh") will now be displayed in the **Voice** field.

### Step 8: Regenerate Your Video

With your ElevenLabs voice selected, you are ready to regenerate your video's voiceover.

Scroll down to the bottom of the "Regenerate Video" modal.

Click the **Regenerate Video** button. Clevera will begin processing your request, generating a new voiceover using the chosen ElevenLabs voice and the specified video settings.

A small chat icon may appear at the bottom right corner of the screen, indicating that the generation process has started. Depending on the video's length and complexity, this process may take some time. Once complete, your video will feature the newly generated ElevenLabs voiceover.

> [!WARNING]
> If the regeneration fails or the voice sounds incorrect, double-check that the stored ElevenLabs API key in **Account Settings** has the required permissions and that your ElevenLabs subscription covers the selected voice.

---

## Conclusion

Congratulations! You've successfully integrated ElevenLabs with Clevera, a significant step towards creating more professional and personalized video content. By generating an API key with the correct permissions in ElevenLabs and then securely linking it within Clevera's account settings, you've unlocked a powerful voice engine for your projects. You can now effortlessly regenerate your video voiceovers, choosing from a wide array of high-quality ElevenLabs voices to perfectly match your brand's tone and message.

This integration empowers you to produce product videos with unparalleled audio quality, enhancing viewer engagement and making your tutorials, demos, and announcements more impactful. Experiment with different ElevenLabs voices to find the perfect auditory identity for each of your videos. Remember — successful integration hinges on correct API permissions and a verified key in Clevera.

> [!TIP]
> Well done — with ElevenLabs connected, you now have access to highly customizable, professional AI voices right inside Clevera.

## FAQ

- **Why do I need specific permissions for the ElevenLabs API key?**
Clevera requires specific read and write access to ElevenLabs services (like Text-to-Speech, Voices, Models, and User data) to properly fetch voices, generate audio, and verify your account status. Granting only necessary permissions is a security best practice.
- **What if my ElevenLabs API key says "Invalid" in Clevera?**
If your key is marked as "Invalid" or shows permission errors, revisit the ElevenLabs Developers > API Keys page. Ensure you have enabled "Access" for Text-to-Speech and "Read" permissions for Voices, Models, and User endpoints, then re-copy and paste the key into Clevera.
- **Can I use different ElevenLabs voices for different videos?**
Absolutely. Once ElevenLabs is configured as a voice engine in Clevera, you can select any of the available ElevenLabs voices from the dropdown menu each time you choose to regenerate a video's voiceover, allowing for flexible customization across your projects.


