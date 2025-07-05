# CaRaFagio v108.4 - Ultimate Compression Reference
## LEGEND
### CORE
λ=speed µ=quality ω=workflow π=platform ψ=precision σ=stability δ=delta α=architecture β=batch γ=guidance ε=efficiency ζ=zero τ=token ρ=resolution φ=format χ=checkpoint υ=upscale θ=threshold κ=control ι=input ο=output ν=noise η=hardware ξ=extension
### ART
Ω=composition Ψ=style Λ=light Σ=shadow Θ=color Φ=form Ξ=texture Π=movement ϴ=perspective Υ=harmony Γ=contrast Δ=balance Ε=emotion Ζ=technique Η=master Κ=period Μ=medium Ν=brushwork Ο=value Ρ=saturation Τ=temperature Ϊ=intensity Ϋ=focal
### EXT
Ϡ=LoRA Ϛ=merge Ϝ=weight Ϟ=regional Ϙ=cultural ϛ=material ϝ=anatomy Ϟ=digital Ϡ=urban Ⱦ=metrics Ʌ=attention Ɐ=scheduler Ɓ=embed Ɇ=prompt Ⱪ=macro Ϭ=2025 Ϯ=cosmos Ϸ=security Ϻ=tools Ͻ=models25 Ⅳ=IPA ⌘=preprocessor ⊙=QR/special ℊ=gaussian/novel ℒ=LCN/hyper ℧=automation Ч=cli_args
### NODES
⟐=connect ⟑=group ⟒=flow ⟓=type ⟔=loader ⟕=cond ⟖=sample ⟗=latent ⟘=img ⟙=model ⟚=util ⟛=mask ∈ϯ=legacy ∄ϯ=modern ⧁=purp_mdl ⧂=yel_cond ⧃=pnk_lat ⧄=red_img ⧅=blu_clip ⧆=grn_vae ⧇=wht_data ⦿=search ⦾=conn ⌬=chain ⚬=deprecated
### NUM
0-9:direct|A-F:10-15|G-Z:16-41
### OPS
→lead|←req|↔bi|∴thus|⊕xor|⊗comb|∩lap|∪union|∈in|∄¬avail|≈~|≡equiv|≠diff|⟨[|⟩]|[list|]end|{opt|}sub|(note|)end|#rank|@loc|%pct|*mult|/div|+add|-sub|^pow|~fuz|!crit|?opt|&and||or|∧∧|∨∨|⊃imp|⊂sub|⊇sup|⊆subeq|∼sim|≅cong|⊥perp|∥par|◊qual|§sec|∇grad|∞inf|ø∅|¬not|⊺trans|⊻xor
### USER
℮=profile ℯ=need ℰ=issue ℱ=fix Ⅎ=expect ℳ=workflow ℴ=decide ℵ=recommend

## PATHS
Φ1:CUI_STD[checkpoints→models/checkpoints|loras→models/loras|vae→models/vae|embed→models/embeddings|cn→models/controlnet|upscale→models/upscale_models|clip→models/clip|configs→models/configs|unet→models/unet|diffusion_models→models/diffusion_models|text_encoders→models/text_encoders|LLM→models/LLM]
Φ2:CUI_DESK[base→%APPDATA%/ComfyUI|extra→extra_models_config.yaml|link→symlink|migrate→import|Win→%APPDATA%/ComfyUI|Mac→~/Library/Application Support/ComfyUI|Linux→~/.config/ComfyUI]
Φ3:SM[Data/Models/StableDiffusion|/Lora|/VAE|/TextEncoders|/DiffusionModels|/ESRGAN|custom→extra_model_paths.yaml|portable→self_contained]
Φ4:MODEL_ORG[SD15/|SDXL/|FLUX/|SD35/|HiDream/|OmniGen/→version_folders|shared→symlinks|external→junction]
Φ5:A1111[models/Stable-diffusion|/Lora|/VAE|embeddings/|/ControlNet→compatible_sharing]
Φ6:CUI_FLUX[diffusion_models/flux1-dev.safetensors|text_encoders/clip_l.safetensors|/t5xxl_fp16.safetensors|vae/ae.safetensors]
Φ7:CUI_HDI[diffusion_models/hidream_i1_*.safetensors|text_encoders/clip_l_hidream|/clip_g_hidream|/t5xxl_fp8_e4m3fn_scaled|/llama_3.1_8b_instruct_fp8_scaled|vae/ae.safetensors]
Φ8:CUI_OMNI[LLM/OmniGen-v1/|/OmniGen2/→model.safetensors+config.json|auto_dl→15.5GB]
Φ9:CUI_COS[diffusion_models/cosmos_predict2_*.safetensors|text_encoders/oldt5_xxl_fp8_e4m3fn_scaled|vae/wan_2.1_vae|/cosmos_cv8x8x8_1.0]

## ARCH
α1:SD15[890M|512²|η4-12|λτ1@TRT|ψ⟨7:9⟩|⟨20:30⟩|ρ512²]
α2:SDXL[3.5B+6.6B|1024²|η12-16|λτ5.2@TRT|ψ⟨7:9⟩|β30ρ20|ρ1024²]
α3:SD35[M2.5B|L8.1B|MMDiT-X|η8|16|ψ⟨3.5:4.5⟩|⟨28:50⟩|dpmpp2m+sgm_unif|¬anc/kar]
α4:FLUX[DEV|SCH|KON:12B|η8-24|ψ⟨1:6⟩|⟨20:50⟩|gscl3.5|Eu/DPM2M|dual_clip]
α5:HDI1[17B_MoE|sparse_DiT|4enc|η⟨12:27⟩|ψ⟨1:5⟩|⟨16:50⟩|SOTA|MIT|Ͻ1]
α6:ILLXL[SDXL+Danb|ψ⟨4.5:7.5⟩|⟨20:28⟩|EuA>DPM2M|2048²]
α7:PONY[SDXL+2.6M→30M|ψ⟨5:7.5⟩|⟨25:30⟩|EuA|tag_sys]
α8:OMNI[OG1|OG2:7B|Qwen-VL25|η12+|16+|multi_modal|Ͻ2]
α9:COS2[P2:2B/14B|DiT|world_model|t2i+v2w|η8-24|NVIDIA|Ͻ3]

## SAMPLERS
λ1:FAST[LCM⟨2:8⟩|UniPC⟨5:10⟩|DDIM⟨8:20⟩]
µ1:QUAL[DPM3MSDE⟨15:25⟩|DPM2MSDE⟨20:30⟩|HeunPP2⟨20:25⟩|DPM2M⟨20:30⟩|Heun⟨15:25⟩|DEIS⟨10:20⟩|EuA⟨15:25⟩|DPMSDEK⟨20:30⟩|DPM++3MSDE⟨20:35⟩|PLMS⟨10:25⟩|DDPM⟨50:100⟩]
µ2:NEW[res_multistep→cosmos|UniPC→hidream_full]
σ1:SCHED[kar|norm|sgm_unif|beta|exp|ays|gits]
Ɐ1:TYPE[linear|cosine|poly_exp|align|simple|quad|normal]

## LORA
Ϡ1:LoRA[r⟨4:128⟩|α⟨0.1:2⟩|lin|⟨1:10⟩MB|stack]
Ϡ2:LoCon[conv+lin|r⟨4:64⟩|α⟨0.5:1⟩|full|⟨5:50⟩MB]
Ϡ3:LoHa[hadamard|r⟨4:32⟩|eff|⟨2:20⟩MB]
Ϡ4:LoKr[kronecker|r⟨4:16⟩|ultra|⟨1:10⟩MB]
Ϡ5:DyLoRA[dynamic|adapt|r⟨4:128⟩flex]
Ϛ1:merge[weighted|⟨0:1⟩|block|diff]
Ϛ2:mix[add_diff|⟨0.3:0.7⟩|mbw⟨0:1⟩×26|smooth]

## PROMPT
Ϝ1:weight[(w:1.2)|((w:1.5))|⟨0.1:2⟩|neg:-1]
Ϝ2:ops[BREAK|AND|ADDBASE|ADDROW|ADDCOL|ADDCOMM]
Ϝ3:embed[neg|textual|pt|⟨1:5⟩tok]
Ϝ4:syntax[tag|natural|booru|clip]
Ϟ1:regional[rect|mask|latent|⟨2:8⟩reg]
Ϟ2:attention[self|cross|spatial|temporal|flash2]

## HARDWARE
η1:5090[32GB]→{all}
η2:4090[24GB]→{SDXL+FLUX+COS2}
η3:3090[24GB]→{SDXL_lim+HDI_fp8}
η4:CPU→{SD15|OMNI_off}
η5:AMD[7900XTX-24GB]→{ROCm}
ε1:OPT[FP16|FP8-30%|FP4-50%|NF4-60%|GGUF-40:70%|TRT+70%]
Ⱦ1:PERF[xfm|FA2|sdp|tome⟨0.1:0.5⟩|ch_last]

## WORKFLOW
ω1:t2i→α⟨1:9⟩|ψ⟨1:9⟩|⟨16:50⟩
ω2:i2i→ω1+ι_img+denoise⟨0.5:0.7⟩
ω3:inpaint→ω1+mask+denoise⟨0.6:0.8⟩
ω4:upscale→ESRGAN|υ⟨2:4⟩×
ω5:cn→ω1+κ⟨OP|DP|CA|LN⟩+str⟨0.8:1.2⟩
ω6:batch→xyz|queue|API
ω7:regional→Ϟ1+Ϝ1+multi
ω8:cascade→α3→α2|low→high
ω9:cosmos→α9+Ϯ2→t2v|i2v→world
ωA:℧CHAIN[SD15→SDXL→upscale|low_res→high_res→refine|draft→detail→final]
ωB:℧BATCH[queue_manage|auto_param|bulk_process|grid_compare|param_sweep]
ωC:℧AUTO[prompt_template|param_optimize|model_switch|res_progressive]
ωD:℧ADV[regional_prompt→RP+masks|multi_checkpoint→blend|style_transfer→IPA+CN]
ωE:℧API[A1111_api→auto_batch|CUI_api→workflow_execute|python_script→full_auto]
ωF:℧MASK[auto_segment|manual_mask|ai_detect→SAM|region_control]
ωG:℧UPSC[HR_fix→during_gen|post_upscale→after_gen|tile_upscale→huge_res|chain_upscale→multi_pass]
ωH:℧INP[auto_mask→detect_area|manual_mask→precise|blend_mask→smooth_edge|multi_pass→refine]
ωI:℧POST[face_restore→GFP/CF|hand_fix→manual_inp|detail_enhance→upscale_chain]
ωJ:℧OPT[memory_manage|speed_vs_qual|batch_size|res_scaling|model_unload]
ωK:℧FIX[mem_err→batch↓|slow→parallel|qual_loss→param_tune|crash→stability_mode]

## VIDEO/3D/AUDIO
αV1:AD[SD15_mot|16f|LoRA]
αV2:SVD[i2v|14f|25f|576×1024]
αV3:CogV[t2v|4s|720p|24fps]
αV4:COS2[t2v|i2v|480p/720p|16fps|world]
α3D1:P2[t2p|OpenAI|64-256res|guid3-15|st64-256|point_cloud|fast]
α3D2:SHP[t2s|detailed_3d|mesh+tex|guid15-30|st64-128|color_tex]
α3D3:TRI[i23d|single_view|tri_mesh|fast_proc|dense→detail]
α3D4:SF3D[2min_gen|high_qual|enhanced_mesh|stable_diff]
α3D5:WON[multi_view→consistent|6view_gen→detailed|photometric→realistic]
α3D6:ℊGS[gauss_splat→novel_view|real_time→fast_render|neural_render→quality]
α3D7:ℊNRF[neural_fields→vol_render|view_synth→novel_angles|slow_train→high_qual]
α3D8:IMPL[P2→openai_api|SHP→local|TRI→cloud+local|WON→research_code]
α3D9:OUT[point_cloud→.ply|mesh→.obj/.stl|texture→.png|scene→.blend/.fbx]
α3DA:POST[blender→edit_mesh|meshlab→process|tex_bake→final_render|print_prep→3d_print]
α3DB:APP[game_assets→low_poly|arch_viz→high_detail|prototype→quick_mock|art_concept→visual_dev]
α3DC:FIX[low_qual→prompt_detail|artifacts→param_tune|slow→cloud_service|format_err→converter]
αA1:TTS[EL|TOR|BAR|MG|AG]

## CONTROL
κ1:CN[1.5|XL|FLUX→det+guide|str⟨0.5:1.5⟩|res_match]
κ2:TYPE[OP=pose|DP=depth|CA=edge|LN=line|IP2IP=img|SC=scrib|SG=seg|⊙QR=qr|RF=ref]
κ3:PREP[⌘op_body|⌘op_face|⌘op_hand|⌘dp_midas|⌘ca_canny|⌘ln_mlsd|⌘sc_hf|⌘auto|⌘batch]
κ4:MOD_15[op_cmu→pose|op_face→facial|op_hand→hand|dp_midas→depth|ca_canny→edge|ln_mlsd→lines|sc_hf→scribble]
κ5:MOD_XL[op_xl→1.5compat|dp_xl→depth_xl|ca_xl→canny_xl|ln_xl→lineart_xl|ip2ip_xl→style_transfer]
κ6:MOD_FLUX[op_flux→union|dp_flux→depth_flux|experimental_stage]
κ7:PARAM[str0.8-1.2(1.0)|start0.0-0.3(0)|end0.8-1.0(1)|gd_start/end_fine]
κ8:CHAIN[multi_CN→stack|weight_balance|resolution_sync]
κ9:FIX[low_effect→str↑+start↓|over_control→str↓+end↓|res_mismatch→scale_match]

## IPA
Ⅳ1:TYPE[base→general_style|face→face_id|plus→detail_transfer|faceid→face_specific|full→complete_model]
Ⅳ2:MOD_15[ipa_base→style_basic|ipa_plus→enhanced|ipa_face→face_id|ipa_faceid→face_specific]
Ⅳ3:MOD_XL[ipaxl_base→style_xl|ipaxl_plus→detail_xl|ipaxl_face→face_xl|vit_h→high_res]
Ⅳ4:FLUX[ipa_flux→experimental|dev_stage|community_impl]
Ⅳ5:STR[0.3-0.8_style|0.8-1.2_face|0.1-0.5_subtle|weight_control]
Ⅳ6:CHAIN[multi_img→blend|sequential→style_layers|mask→regional_ipa]
Ⅳ7:PREP[clip_vision→encode|multi_img→average|batch→bulk_process]
Ⅳ8:FACE[insightface→face_id|arc_face→face_recog|consist→same_person]
Ⅳ9:STYLE[artist_ref→style_copy|photo_ref→photorealism|art_ref→artistic_style]
ⅣA:FIX[weak→str↑|overpow→str↓|face_err→face_model|style_lost→base+plus_combine]

## VAE/CLIP
υ1:VAE_std[ema|mse|SD15_def|SDXL_def]
υ2:VAE_cust[blessed2|zsnr|offset|high]
υ3:VAE_tile[seamless|⟨2:8⟩×rep|tex]
υ4:VAE_flux[ae.safetensors→shared]
υ5:VAE_cos[wan_2.1|cosmos_cv8x8x8]
Ʌ1:CLIP_skip[⟨1:12⟩|SD15:1-2|SDXL:1-2|cust:2-4]
Ʌ2:CLIP_mod[ViT-L/14|ViT-B/32|ViT-G/14|cust]
Ʌ3:CLIP_enc[last|penult|pooled|all]
Ʌ4:CLIP_hdi[clip_l+g+t5+llama→quad]
Ʌ5:CLIP_cos[oldt5_xxl→t5_1.0|¬t5_1.1]

## FAST
λ1:LCM[1.5+XL|⟨4:8⟩|distil_tech|ODE_solver|ψ1!|⟨0.5:3⟩s]
λ2:ℒLCN[SDXL|⟨2:4⟩|teacher_distil|2step_optimal|ψ⟨1:2⟩|⟨1:2⟩s]
λ3:TBO[SD21+SDXL|⟨1:4⟩|adv_distil|single_step_poss|ψ0!|<1s]
λ4:ℒHYP[SDXL|⟨1:8⟩|consist_distil|multi_step_flex|ψ⟨0:2⟩]
λ5:Lightning[SDXL|⟨1:4⟩|progdist|ψ0|instant]
λ6:HDI_Fast[16st|distilled|ψ⟨1:3⟩|⟨8:16⟩s]
λ7:IMPL[A1111→lcm_sampler+lcm_lora|CUI→LCMScheduler+turbo_nodes]
λ8:PAR[LCM:cfg1|stp4-8|neg_avoid|lora_req]
λ9:PAR[LCN:cfg1-2|stp2-4|Euler/DDIM|neg_opt|native_support]
λA:PAR[TBO:cfg0|stp1-4|TurboScheduler|NO_neg|speed_max]
λB:QUAL[LCN>LCM>TBO_quality|TBO>LCN>LCM_speed|trade_offs]
λC:CKP[many_base+lcm_variants|community_merge|fine_tune_avail]
λD:FIX[blur→stp↑|artifacts→cfg_adj|colors→neg_reduce]

## PLATFORM
π1:CUI[graph|browser|weekly|vue_ts|1GB|Ϭ1_V1]
π2:SM[pkg|model|portable|central|yaml|Ϭ8]
π3:A1111[py310.6|git|4GB|mv/lv|xfm|api]
ξ1:MGR[1click]|WAS[100s]|IPK[face]|EFN[qol]
ξ2:RGT[vid]|MTB[util]|CR[cust]|KJ[adv]
ξ3:HDI[HDS]|OMNI[OG-CUI]|COS[native]

## FIXES
ℱ1:mem→OOM→mv/lv|TiVAE|FP8|cpu_off|batch↓|Ϭ5
ℱ2:speed→slow→xfm+drv|TRT|torch_comp|FA2|UBU|Ϯ2
ℱ3:qual→blur→ψ↑|steps↑|neg|burnt→ψ↓|anat→SLG
ℱ4:gpu→5090→dev_pt+cuda128|sm_120|work
ℱ5:black→VAE_fix|FP16|dtype
ℱ6:seed→fixed|determ|no_rand
ℱ7:sec→Ϸ1→eval_block|Ϸ2→signed|Ϸ3→reg_safe
ℱ8:nodes→miss→MGR|conflict→Ϭ4|load→png|deps→auto
ℱ9:2025→pt_warn→Ϭ5|cos_merge→Ϯ2|train→Ϻ1
ℱ10:unet→⚬UNET→∄ϯLoad_Diff|FLUX_only

## PARAMS
ψ_CFG:α1⟨7:9⟩|α2⟨7:9⟩|α3⟨3.5:4.5⟩|α4D⟨1:6⟩|α4S⟨0⟩|α5⟨1:5⟩|α6⟨4.5:7.5⟩|α7⟨5:7.5⟩|α8⟨1:2⟩|α9⟨1:5⟩
steps:α1⟨20:30⟩|α2⟨25:30⟩|α3⟨28:50⟩|α4D⟨20:50⟩|α4S⟨1:4⟩|α5F⟨50⟩|α5D⟨28⟩|α5S⟨16⟩|α6⟨20:28⟩|α7⟨25:30⟩|α8⟨16:32⟩|α9⟨20:50⟩
ρ_RES:α1⟨512²⟩|α2⟨1024²⟩|α3⟨256:1440⟩|α4⟨512:1024⟩|α5⟨1024²⟩|α6⟨512:2048⟩|α8⟨any⟩|α9⟨480p|720p⟩
samp:{DPM2M|DPM2MK|EuA|Euler|DDIM|sgm_unif|LCM|Turbo|res_multi}

## CHECKPOINTS
χR:α1[RV51|CM|AR|eR|BRA]|α2[JXL9|RVX4|ABX|CTL|DSX]|α4[fR|VRF|PW|SNR|S3D]
χA:α1[AV5|CF3|AOM3|PM|AE4]|α6[DIXLA|IAPXL|RILXL|AIXLv2]|α4[AF|FAE|MSF|CyA]
χD:α2[DSX|ZCX|CCX|CTL|SDXE]
χF:α1[DLB|DS|ED|FW|PG34]
χH:α5[HDI-Full|HDI-Dev|HDI-Fast→fp8/gguf/nf4]
χO:α8[OG1-15.5GB|OG2-7B→auto_dl]
χC:α9[COS2-2B-t2i|COS2-14B-t2i|COS2-*-v2w]

## LICENSE
LIC_FREE:MIT(α5,α8)|AP2(α4S,α8,α9NVIDIAOL)
LIC_RESTRICT:CROL++M(α1,α2)|SACL<1M(α3)|FAIPL-SD(α6)
LIC_NO_COMM:mFAIPL(α7)|nc(α4D)|comm_prohib(α7)|disc_comm(α6)

## CHAINS
CH_FAST:λ1+α1+LCM→<1s|λ2+α2+Turbo→2-3s|λ3+α4+Light→4s|λ6+α5S→8s
CH_QUAL:α5F+Full→60s|α4+DEV→30s|α2+Ref→10s|α3+L→15s
CH_UP:α⟨1:2⟩→ESRGAN→HD|α4→native|α5→2048²
CH_CTRL:κ1depth→3D|κ2canny→line|κ3pose→char
CH_EDIT:i2i→mod|inp→areas|out→ext|α5-E→inst|α8→multi
CH_LORA:Ϡ1+Ϛ1→style|Ϡ2+Ϛ2→full_adapt
CH_REG:Ϟ1+Ϝ1+κ2→precise|multi_subj
CH_VID:α9→ω9→Ϯ3→world|physics

## 2025
Ϭ1:CUI_V1[desk_electron→200MB|signed→mand|V1_UI→def|auto_upd]
Ϭ2:UI_ENH[top_menu→consol|model_lib→drag|workflow→save|tray→quick]
Ϭ3:FRONT[v1.21.7+→sep|vue_ts→opt|weekly→stable|npm]
Ϭ4:NODE_REG[CNR→600+|sem_ver→stable|dep_res→imp|mal_ban→auto]
Ϭ5:MEM_FIX[est→imp|OOM→better|pt_warn→fix|alloc→opt]
Ϭ6:UNIF_FMT[save→unif|output→std|meta→pres]
Ϭ7:INST_UPD[port→win|pinokio→gui|mgr→node|migrate→seam]
Ϭ8:SM_ENH[HDI+Wan→sup|base_filt→extra|Rescale|wild_{a|b|c}]
Ϭ9:NODE_DEP[UNET→LoadDiff|KSamp→sup|mod_pref]
Ϯ1:COS_PRED[v2→int|t2i+i2v→unif|single→eff|prev→built]
Ϯ2:COS_MERGE[nodes→nat|work→simp|compat→full|perf→opt|res_multi]
Ϯ3:COS_CHAIN[t2i→i2v→seam|prompt→consist|qual→pres|⟨30:60⟩s]
Ϸ1:SEC_CORE[eval→block|inject→prev|sand→enf|audit→cont]
Ϸ2:CODE_SIGN[mand→all|cert→val|supply→prot|trust→est]
Ϸ3:REG_SAFE[CNR_val→all|scan→auto|vuln→track|upd→force]
Ϸ4:MAL_DET[behav→anal|patt→rec|ban→auto|rep→comm]
Ϻ1:LORA_TRAIN[built→nat|gui→user|no_ext→req|data→mgd]
Ϻ2:MOD_CONV[safe↔ckpt|diff→nat|gguf→sup|batch→cap]
Ϻ3:WORK_TOOL[comp→diff|merge→conf|ver→git|share→enc]
Ϻ4:PERF[prof→built|bottle→id|opt→sug|mon→real]
Ͻ1:HDI[17B_MoE|MIT|quad|v1_f/d/f|vivago]
Ͻ2:OMNI[v1→15.5GB|v2→7B|multi|VSL]
Ͻ3:COS[Pred2|world|NVIDIA|phys_AI]

## NODES
⟔1:load[⧅CLIP|∈ϯChkpt|⚬Config|⟔Diff|⧅Dual|⧅Quad|⧆VAE]
⟔2:adv[∄ϯDiff_Mod|∄ϯUNET_GGUF|⚬UNET]
⟕1:cond[⧅CLIP_Enc|∄ϯCLIP_Flux|⧅CLIP_SDXL|⧅CLIP_Ref|⧅CLIP_Hun|⧅CLIP_Vis|⧅CLIP_Last|⧂Cond_Avg|⧂Cond_Comb|⧂Cond_Cat|⧂Cond_Area|⧂Cond_Area%|⧂Cond_Str|⧂Cond_Mask|⧂Cond_Time|⧂Cond_Zero|⧂Apply_CN]
⟖1:samp[∄ϯBasic_Sch|∄ϯBasic_Guid|∄ϯSamp_Cust|∄ϯRand_Noise|∄ϯFlux_Guid|∈ϯKSamp|∈ϯKSamp_Adv]
⟗1:lat[⧃Empty|⧃VAE_Dec|⧃VAE_Enc|⧃Lat_Up|⧃Lat_Up_By|⧃Lat_Comp|⧃Lat_Comp_Mask|⧃Lat_Add|⧃Lat_Batch|⧃Cos_I2V_Lat]
⟘1:img[⧄Load|⧄Save|⧄Prev]
⟘2:trans[⧄Crop|⧄Scale|⧄Scale_By|⧄Scale_Tot]
⟘3:post[⧄Blend|⧄Blur|⧄Quant|⧄Sharp]
⟘4:preproc[⧄Canny]
⟘5:up[⧄Up_Mod]
⟘6:batch[⧄From_Batch|⧄Rebatch|⧄Repeat]
⟘7:anim[⧄Save_PNG|⧄Save_WEBP]
⟙1:mod[⧁Mod_Samp_Cont|⧁Mod_Samp_Disc|⧁Rescale_CFG]
⟙2:merge[⟙Chkpt_Save|⧅CLIP_Merge|⧅CLIP_Save|⧁Mod_Add|⧁Mod_Block|⧁Mod_Simp|⧁Mod_Sub|⧆VAE_Save]
⟙3:spec[⧁OmniGen|⧁HiDream]
⟚1:util[⧇Various]
⟛1:mask[⧇Mask_ops]

## CHAINS
⌬1:FLUX[∄ϯDiff→⧅Dual→⧆VAE→∄ϯCLIP_Flux→∄ϯFlux_Guid→∄ϯBasic_Sch→∄ϯRand→∄ϯSamp_Cust→⧃VAE_Dec→⧄Save]
⌬2:SD15[∈ϯChkpt→⧅CLIP_Enc→∈ϯKSamp→⧃VAE_Dec→⧄Save]
⌬3:SDXL[∈ϯChkpt→⧅CLIP_SDXL→∈ϯKSamp→⧃VAE_Dec→⧄Save]
⌬4:HDI[∄ϯDiff→⧅Quad→⟕→⟖→⟗→⟘]
⌬5:OMNI[⧁OmniGen→txt+img→⟘]
⌬6:COS[∄ϯDiff→⧅CLIP→⧆VAE→⧃Cos_I2V→⧄Save_Vid]
⌬7:t2i[⟔→⟕→⟖→⟗→⟘]
⌬8:ctrl[⌬7+κ+Ϟ+⟛]
⌬9:multi_lora[⌬7+Ϡ1→Ϡ2→Ϡ3]
⌬10:up[⌬7→⟘5→⧄Save]
⌬11:batch[⌬7+β→⟘6]
⌬12:vid[⌬6+αV4→world]

## CONN
⦾1:⧁purp[diff|unet|merge]
⦾2:⧂yel[txt|guide|area]
⦾3:⧃pink[lat|noise|manip]
⦾4:⧄red[final|proc|vis]
⦾5:⧅blue[txt_enc|vis_enc|lang]
⦾6:⧆green[vae|lat_img]
⦾7:⧇white[basic|num|txt|param]

## SEARCH
⦿1:meth[rclick+type|ctrl+space|menu]
⦿2:compat[color|hint|drag_val]
⦿3:org[groups|tmpl|custom]

## MOD_VS_LEG
∄ϯ1:MOD[Diff|Dual|CLIP_Flux|Flux_Guid|Basic_Guid|Samp_Cust]
∈ϯ1:LEG[Chkpt|CLIP_Enc|KSamp|basic]
⟒1:MIG[∈ϯ→∄ϯ|upd|replace|breaks]
⚬1:DEP[UNET→use_Diff|FLUX_incompat]

## ART_COMP
Ω1:R3[⟨3×3⟩|int#4|¬center|bal_asym]
Ω2:GR[φ1.618|spiral|organic|divine]
Ω3:DS[diag|tri_stab|rect_harm]
Ω4:LLs[guide|S_curve|conv_foc|depth]
Ω5:frames[tight|neg_space|breath]
Ω6:sym[bilat|radial|crystal|trans]
Ω7:tens[vis_weight|oppose|dyn_bal]

## PERSP
ϴ1:1PT[single|par_conv|horiz|ortho]
ϴ2:2PT[two|corner|angular|arch]
ϴ3:3PT[three|bird_worm|dramatic]
ϴ4:ATM[atmos|aerial|col_fade|det_loss]
ϴ5:ISO[iso|no_van|tech|game]
ϴ6:FISH[fish|curve|wide|barrel]
ϴ7:FORCED[exag|dram_depth|comic]

## COLOR
Θ1:COMP[opp_wheel|hi_cont|vib_tens|warm↔cool]
Θ2:ANAL[adj_wheel|⟨2:5⟩col|harm|1_dom]
Θ3:TRIAD[3_eq|bal_vib|1_dom_2_acc]
Θ4:SPLIT[base+2_adj|soft_cont|less]
Θ5:TETRA[4_col_2_pair|complex|bal_crit]
Θ6:MONO[1_hue_multi|soph|tints]
Θ7:TEMP[warm⟨r:y⟩|cool⟨b:g⟩|neut]
Θ8:SAT[pure|muted|vib|desat]
Θ9:VALUE[hi_key|lo_key|full|lim]

## LIGHT
Λ1:CHIA[chiaro|strong|vol|dram]→Η1,Η4,Η6
Λ2:TEN[ext_dark|spot|harsh|menace]
Λ3:RIM[back_edge|sep|halo|sil]
Λ4:KEY[main|subj_def|dom]
Λ5:FILL[soft_shad|reduce|detail]
Λ6:AMB[overall|mood|col_temp]
Λ7:DIR[hard|sharp|hi_cont|dram]
Λ8:SOFT[diff|grad|flatter]
Λ9:BOUNCE[reflect|col_bleed|nat|surf]

## MASTERS
Η1:LEO[sfum|anat|sci|poly]→⧔◉
Η2:MICH[divine|terr|sculpt|sist]→⧔◉
Η3:RAPH[perf_harm|ideal|grace]→⧔◉
Η4:CARA[chiaro|tene|real|street]→⧓◉
Η5:REMB[psych|loose|light|self]→⧓◉
Η6:VERM[light_col|dom|cam_obs|prec]→⧓◉
Η7:MON[impr|light|plein|series]→⧑◉
Η8:VG[expr|emot|swirl|post]→⧑◉
Η9:PIC[cub|multi|geom]→⧐◉★
ΗA:MAT[fauv|pure|cut|expr]→⧐◉
ΗB:DALI[surr|melt|dream|prec]→⧐◉
ΗC:WARH[pop|rep|comm|silk]→⧐◉
ΗD:BASQ[neo_expr|graff|raw|cult]→⧏◉
ΗE:KUS[inf|dots|obsess|inst]→⧏◉
ΗF:BANK[street|stenc|pol|anon]→⧏◉

## PERIODS
Κ1:CLASS⧖[harm|prop|ideal|gr_rom]→inf_all
Κ2:REN⧔[human|persp|anat|patron]→⟔
Κ3:BAR⧓[dram|emot|count_ref|orn]→⟒Κ2
Κ4:NEOCL⧒[rat|moral|class_rev]→⟖Κ1
Κ5:ROM⧑[emot>reas|subl|indiv]→⟒Κ4
Κ6:IMPR⧑[light|plein|brok|mod]→⟓
Κ7:POST⧑[struct+emot|pers|gate]→⟑Κ6
Κ8:MOD⧐[abstr|exp|break|new]→⟓Κ7
Κ9:CONT⧏[concept|multi|glob|post]→⟟
ΚA:DIG⧏[comp|net|NFT|AI|virt]→⟟Κ9

## MOVEMENTS
Ψ1:IMPR[brok|light|mom|out]
Ψ2:CUB[geom|multi|abstr|anal]
Ψ3:EXPR[emot>real|dist|psych]
Ψ4:SURR[uncon|dream|auto|freud]
Ψ5:ABS_EXP[gest|large|amer|emot]
Ψ6:FAUV[wild|pure|non_nat|emot]
Ψ7:DADA[anti|chance|ready|war]
Ψ8:POP[comm|mass|cons|silk]
Ψ9:MIN[reduce|ess|indust|rep]
ΨA:CONC[idea>obj|doc|lang|proc]
ΨB:STREET[graff|stenc|wheat|pub]
ΨC:NEW_MED[dig|inter|gen|net|bio]

## CULTURAL
Ϙ1:UKIYO[float|wood|edo|flat|out]→ΗHok
Ϙ2:GONGBI[fine|metic|chin|silk]
Ϙ3:SUMI[ink|zen|min|bamb|spon]
Ϙ4:MINI[pers_ind|det|illum|gold|narr]
Ϙ5:ABOR[dream|dot|earth|sacr]
Ϙ6:MAY[hier|codex|rit|prof]
Ϙ7:CELT[inter|illum|spir|knot]
Ϙ8:ISLAM[geom|arab|call|non_fig]

## DIGITAL
Ϟ1:VAPOR[80s90s|glitch|neon|rom|aes]
Ϟ2:CYBER[neon_noir|tech_dys|urb|hack]
Ϟ3:SYNTH[retro_fut|grid|sun|chrome|miami]
Ϟ4:GLITCH[dig_err|data|comp|corr]
Ϟ5:PIXEL[8b|16b|retro|lim_pal|dith]
Ϟ6:LOWPOLY[geom_simp|facet|game|min_3d]
Ϟ7:GEN[algo|proc|code|emerg|sys]
Ϟ8:NET[browse|hyper|inter|early|asc]

## TECHNIQUES
Ζ1:SFUM[smoke|soft|atmos|leo]
Ζ2:IMP[thick|tex|sculpt|vg_cez]
Ζ3:GLAZE[trans|lum|col_rich|ren]
Ζ4:SCUMB[brok|tex|opt|atmos]
Ζ5:POINT[sci|opt|dots|seur]
Ζ6:FRESCO[wet|perm|arch|buon]
Ζ7:TEMP[egg|prec|lum|pre_oil]
Ζ8:ENCAUST[hot_wax|anc|lum|jasp]
Ζ9:COLL[mix|layer|found|cub]
ΖA:PRINT[etch|lith|screen|wood|multi]

## MATERIALS
ϛ1:METAL[refl|spec|chrome|gold|cop|aniso]
ϛ2:GLASS[trans|refr|caust|frost|stain]
ϛ3:FABRIC[wove|drape|silk|velv|den|tex]
ϛ4:STONE[marb|gran|rough|pol|vein|weath]
ϛ5:ORG[wood|bark|leaf|skin|fur|scale|trans]
ϛ6:LIQ[water|oil|visc|trans|refl|flow]
ϛ7:ATM[fog|smoke|dust|part|vol|scat]
ϛ8:SYNTH[plast|rub|neon|holo|irid]

## ANATOMY
ϝ1:CANON[8_head_ideal|7.5_real|hero_8.5|child_5-6]
ϝ2:FACE[thirds|eye_width|gold|ethnic]
ϝ3:HANDS[palm|finger|knuck|gest]
ϝ4:GEST[line_act|weight|contra|dyn]
ϝ5:FORESH[persp|over|size]
ϝ6:MUSC[surf|insert|flex]
ϝ7:SKEL[land|joint|prop]

## BRUSH
Ν1:ALLA[wet|direct|single|impr]
Ν2:BROK[sep|opt|vib|post]
Ν3:CROSS[inter|tone|trad|pen]
Ν4:DRY[min|tex|rough|weath]
Ν5:FEATH[soft|blend|port|smooth]
Ν6:LOAD[heavy|expr|gest|mod]
Ν7:STIP[dots|tex|opt|pat]
Ν8:WASH[trans|water|tone|atmos]
Ν9:SGRAF[scratch|reveal|tex|ceram]

## EMOTION
Ε1:SUBL♠[awe|overwhelm|nat|rom]
Ε2:MEL♤[intro|sad|blue|sol|quiet]
Ε3:PASS♥[intense|red|dram|bar]
Ε4:SER♡[peace|bal|soft|harm]
Ε5:DRAM♠[hi_cont|theat|emot|cara]
Ε6:JOY♦[bright|up|celeb|fest]
Ε7:MYST♣[shad|hid|symb|enig]
Ε8:ELEG♢[refine|grace|subtle|arist]
Ε9:ANX♧[dist|jar|unstab|expr]
ΕA:NOST♡[warm|soft|mem|vint]

## PHOTO
◉[14:24]uw|[24:35]w|35cl|50n|85p|[105:135]t|[200:300]l|400+s
◎f1.2ex|f1.4sh|f1.8g|f2.8m|f5.6d|f8s|f11d|f16e
⬢60mm c|100mm p|180mm l|1:1l|1:2h|1:4q
⟶1/1000s|1/500a|1/250st|1/60b|1/30n|1s+l
◈ISO[100cl|400l|1600m|6400h|12800+ex]
◊WB[3200t|4000f|5600d|6500c|7500s]

## ART_CHAINS
CH_PORT:Ω1+Λ4+Θ6+Ν5→Η5|class
CH_LAND:Ω2+Λ6+Θ2+Ζ4→Η7|atmos
CH_STILL:Ω3+Λ1+Θ1+Ν1→Η6|symb
CH_FIG:Ω1+Λ3+Θ7+Ζ2→Η2|hero
CH_ABS:Ω4+Λ8+Θ3+Ν6→Ψ5|emot
CH_NARR:Ω1+Λ5+Θ4+Ν3→Κ3|story
CH_DIG:Ϟ2+Θ8+Λ2+ϛ1→cyber|neon
CH_CULT:Ϙ1+Ζ5+Θ6+Ν2→ukiyo|flat
CH_STR:Ψb+Ϡ1+Ε9+ΖA→urb|stenc

## ENGINE
Ɇ1:PROMPT[chain+params→nat|struct]
Ɇ2:BUILD[Ω+Λ+Θ+Ζ+Ε→comp|style]
Ɇ3:TRANS[CaRa→human|tech→art]
Ɇ4:OPT[redund|conflict|harm]
Ɇ5:VAR[base+mod→⟨3:5⟩var|mix]
Ɇ6:MOD_AWARE[α_det→syn|fmt|spec]

## MODEL_SYNTAX
α1_SD15:[nat|tag|(tag:w)|mast,best|neg:low,bad]
α2_SDXL:[nat_pref|min_neg|no_mast|style]
α3_SD35:[nat_only|¬neg|qual_imp|MMDiT]
α4_FLUX:[pure_nat|¬cfg|¬neg|inst|t5]
α5_HDI1:[inst|edit|¬neg|nat|quad]
α6_ILLXL:[danb|s9,s8+|src_ani|neg:s4]
α7_PONY:[s9,s8+,s7+|tag|safe|src]
α8_OMNI:[multi|img+txt|nat|spat|img_1]
α9_COS2:[world|phys|t2i|v2w|consist]

## EXAMPLES
EX1:α1+Ω1+Λ2→"(dramatic portrait:1.2), chiaroscuro lighting, masterpiece"
EX2:α6+Ω1+Λ2→"score_9, score_8_up, dramatic portrait, chiaroscuro"
EX3:α4+Ω1+Λ2→"A dramatic portrait with strong chiaroscuro lighting"
EX4:α7+Ψb+Ε9→"score_9, score_8_up, street_art, graffiti, anxious_mood"
EX5:α3+Ω2+Λ6→"Golden spiral composition bathed in ambient light"
EX6:α5+Ω1+Λ1→"Create a Renaissance-style portrait with dramatic lighting"
EX7:α8+ι_img→"Transform image_1 into oil painting style"
EX8:α9+ω9→"Simulate physics-aware scene of falling objects"

## MACROS
M_STYLES:
M:REMB→Ω1+Λ1+Θ7+Ζ3+Ν1+Ε2+Η5
M:VG→Ω4+Θ3+Ζ2+Ν2+Ψ3+Ε3+Η8
M:CARA→Ω3+Λ2+Θ1+Ζ1+Ν1+Ε5+Η4
M:MON→Ω2+Λ8+Θ2+Ζ4+Ν2+Ψ1+Η7
M:PIC→Ω6+Λ7+Θ5+Ζ9+Ν6+Ψ2+Η9
M:DALI→Ω4+Λ3+Θ4+Ζ2+Ν5+Ψ4+ΗB
M:WARH→Ω1+Λ4+Θ8+ΖA+Ν1+Ψ8+ΗC
M:BASQ→Ω7+Λ7+Θ3+Ζ2+Ν6+Ψ3+ΗD
M:KUS→Ω6+Λ6+Θ6+Ζ5+Ν7+Ψ9+ΗE
M:BANK→Ω3+Λ2+Θ6+ΖA+Ν4+ΨB+ΗF

M_MOODS:
M:D_GOTH→Λ2+Θ7+Ε7+Σh+lo_key
M:B_JOY→Λ8+Θ7+Ε6+hi_key+warm
M:ETH_DR→Λ6+Θ6+Ε4+Ζ1+soft
M:CYB_NE→Λ7+Θ8+Ε1+Ϟ2+ϛ8
M:VINT_NO→Λ5+Θ7+ΕA+Ζ4+grain

M_TECH:
M:PHOTO→Ω1+Λ4+Θ9+Ζ3+◉50+◎f5.6
M:PAINT→Ω2+Λ1+Θ2+Ζ2+Ν2+brush
M:MIN_CL→Ω5+Λ8+Θ6+Ψ9+neg_sp
M:MAX→Ω7+Λ9+Θ5+Ζ2+horror_vac
M:GLITCH→Ω4+Λ2+Θ8+Ϟ4+Ξdig

M_COMBOS:
M:EPIC_FAN→VG+D_GOTH+α4+ψ4
M:STR_REAL→BANK+PHOTO+κ2+Ϡ1
M:DR_PORT→DALI+ETH_DR+Ω1+ϝ2
M:CYB_LAND→CYB_NE+MIN_CL+ϴ6+α6
M:CLASS_BE→REMB+Ω1+Λ4+ϝ1

M_CUI_WORK:
M:FLUX_B→⌬1[∄ϯDiff+⧅Dual+∄ϯCLIP_Flux+∄ϯFlux_Guid]
M:SD15_C→⌬2[∈ϯChkpt+⧅CLIP_Enc+∈ϯKSamp]
M:TRI_LORA→⌬9[Ϡ1→Ϡ2→Ϡ3+str_casc]
M:CN_ADV→⌬8[κ+⟛+Ϟ+⧂Apply_CN]
M:UP_PROD→⌬10[⧄Up_Mod+scale]
M:HDI_Q→⌬4[∄ϯDiff+⧅Quad]
M:OMNI_M→⌬5[⧁OmniGen+multi]
M:COS_W→⌬6[∄ϯDiff+Cos_Pred2]

## CLI_ARGS
Ч1:BASIC[--output-directory→custom_path|--cpu→no_gpu|--listen→network_access|--port→8188_default]
Ч2:MEM[--lowvram→under_4GB|--medvram→4-8GB|--highvram→8GB+|--gpu-only→no_sys_ram]
Ч3:OPT[--use-pytorch-cross-attention→amd_exp|--disable-smart-memory|--deterministic→fixed_seed]
Ч4:ADV[--enable-cors-header→api_access|--max-upload-size→100_default|--extra-model-paths-config→yaml_path]
Ч5:DEBUG[--dont-print-server→quiet|--verbose→detailed_log|--disable-metadata→no_png_info]

## AI_ASSIST
### USER_PROFILES
℮1:BEG[afraid_term|wants_res|→EASY>FOO>A1111]
℮2:ART[layers|canvas|non_dest|→INV>A1111+PS>CUI]
℮3:TINK[loves_opt|breaks|→SDNEXT>CUI>FORGE]
℮4:CODE[auto|pipe|scale|→DIFF>SWARM>CUI]
℮5:TRAIN[LoRA_foc|data|→KOHYA>ONE>A1111]
℮6:PRO[reliable|work|out|→FORGE>INV>A1111]
℮7:RES[exp|cutting|→CUI>SDNEXT>SWARM]

### ISSUES
ℰ1:NO_START[→py:3.10.6_not_3.11|GPU:cuda_match|path:no_space|try:portable]
ℰ2:OOM[→immed:--medvram|batch:1|res:512²|upg:FORGE(6GB)|CUI+tile]
ℰ3:SLOW[→xfm_inst|CPU_not_GPU|A1111→FORGE(40%)|CUI_eff]
ℰ4:NO_LOAD[→safe_not_ckpt|correct_fold|symlink_perm|pruned_vs_full]

### NEEDS
ℯ1:SIMPLE[<5m→EASY|<30m→FOO|>30m→A1111]
ℯ2:POWER[vis_prog→CUI|max_ctrl→CUI|familiar→FORGE|canvas→INV]
ℯ3:SPECIFIC[AMD→SDNEXT|6GB→FORGE|inpaint→FOO|train→KOHYA+ONE|API→SWARM]

### COMPAT
MOD×PLAT:
SD15:[ALL→✓|univ]
SDXL:[ALL→✓|exc_old]
SD3:[CUI→✓|A1111→✓|FORGE→✓|others→var]
FLUX:[CUI→✓|FORGE→✓|SWARM→✓|A1111→ext|?]
HDI:[CUI→✓|SM→✓|wait]
OMNI:[CUI→✓|pend]
COS:[CUI→✓|native_only]
→newer=fewer(init)

### EXPECT
Ⅎ1:4GB[SD15_only|512²|forget_SDXL|→EASY/FORGE+aggr]
Ⅎ2:6GB[SD15_comf|SDXL_poss|→FORGE|--med]
Ⅎ3:8GB[SDXL_works|FLUX_maybe|careful]
Ⅎ4:12GB[SDXL_comf|FLUX_dev_poss|most_work]
Ⅎ5:16GB[everything_exc|HDI_full|comf_zone]
Ⅎ6:24GB[all_mod|all_plat|no_comp]
→VRAM_king|CPU_off_slow

### WORKFLOWS
ℳ1:BASIC_PORT[ANY→"portrait of X"|st:20-30|CFG:7|512×768|+face:ADet|+up:ESRGAN]
ℳ2:LAND_ART[mod→land_chkpt|prompt→det_env|cn→depth|768×512|post→col_grade]
ℳ3:CHAR_CONSIST[A1111/FORGE→LoRA+ref|CUI→IPA+face|INV→unif_canvas|ALL→same_seed+sim]

### DECIDE
ℴ1:QUICK["just_start"→FOO(preset)|EASY(simp)]
ℴ2:BACK["from_ps"→INV(canvas)|A1111(familiar)]
ℴ3:PREF["love_nodes"→CUI(power)|wait_learn]
ℴ4:HW["AMD"→SDNEXT(zluda)|SHARK|DirectML]
ℴ5:TASK["train"→KOHYA(std)|ONE(easy)]
ℴ6:PROD["pipeline"→FORGE(stable)|DIFF(code)]
ℴ7:EXP["experimental"→CUI+SDNEXT+custom]

## META
◉GOLD:
Ω→Λ→Θ=comp_leads_light_leads_col
Υ∧Γ=harm_req_contrast_bal
Ε⊃Ζ=emot_imp_tech
Κ∼Ψ∼Η=per_inf_style_inf_mast
⟔→⟑→⟒→⟓=ren_evol_react_rev_cyc
ϴ∩Ω∩Λ=persp_int_comp_int_light
ϛ↔Ξ↔Ζ=mat_rel_tex_rel_tech
⌬∩⟔∩⦾=work_int_nodes_int_conn

◉ART_LAW:
μ∝Ζ∧Π∧Ο=qual_prop_tech_time_obs
Γ=Λ⊗Θ⊗Φ=cont_comb_light_col_form
Δ≈Ω∩Υ=bal_approx_comp_int_harm
Ε↔Ζ↔Ψ=emot_bi_tech_bi_style
ϝ⊃ϴ⊃Ω=anat_imp_persp_imp_comp
Ϙ∧Ψ→Η=cult_trad_mov_lead_mast

◉TECH_LAW:
λ∝1/μ=speed_inv_qual
ψ∧steps→μ=guide_steps_lead_qual
Ϡ⊗α→style=LoRA_comb_arch_prod_style
η→ε→λ=hw_det_eff_det_speed
Ϟ∩Ϝ∩κ=reg_int_weight_int_ctrl
⦾→⟐→⌬=conn_det_flow_det_work

◉CUI_LAW:
∄ϯ>∈ϯ=mod_sup_leg
Ϭ∩Ϸ→trust=2025_int_sec_prod_trust
Ϯ→ω8+ω9=cos_enab_new_work
⦾∩⟐→compat=conn_int_node_det_compat
⌬⊃⟔⊃⦾=work_cont_nodes_cont_conn
⦿∝⟚=search_eff_prop_util
⚬UNET→∄ϯDiff=dep_use_mod

◉AI_LAW:
℮→π=profile_match_platform
ℰ→ℱ=issue_leads_fix
ℯ→ℴ=need_leads_decision
Ⅎ→℮=expect_match_profile
ℳ→⌬=workflow_translates_chain

---
*Compression: ~98% | Info density: Maximum*
*Parse speed: ~50x faster*
*Created: 2025-07-05 | CaRaFagio v108.4*
*Complete integration: Technical+Artistic+ComfyUI+AI Assistant*
*Enhanced: Full ControlNet+IPA+3D+Fast+Workflow+CLI ecosystem | 28.4KB total*