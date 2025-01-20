# RT_multi-IP-morph
Morphing multiple image prompts using an alpha animation.

Created by FungAI - @orinthesky

This workflow uses multiple embeded image prompts, driven by the movement pattern of an alpha animation.  Using QR Monster V2 you can drive the movement with any alpha animation including real time midi controlled generative sources from tools like Synesthesia Live or Resolume Arena.

The IPadapter Plus node pack is necessary for this.  If you want to run this in ComfyStream, as of now there can only be one "load image" node input in the workflow, so all image prompts must be saved as embeddings and reloaded as such in the workflow.  
I've encluded a worklfow called "IP_embedding_saver" which has everything turned off except a group ready to save your concatenated embeddings. Use this to save your embeds and then move the saved .ipadapter files to the /inputs folder in your ComfyUI folder so the "load IPadapter embeds" node can find them.
