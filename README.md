Manim Math Educational Video Generator - Pseudocode



System Overview


SYSTEM: Manim Math Educational Video Generator


PURPOSE: Generate mathematical animation videos from prompts


ARCHITECTURE: Multi-agent system with code generation, review, and execution

    BEGIN Workflow

        INPUT: user_text_prompt
    
        STEP 1: Code Generation Phase
            CALL CodeBuilder(user_prompt) → raw_manim_code
    
        STEP 2: Code Review Phase  
            CALL CodeReviewer(raw_manim_code) → optimized_manim_code
    
        STEP 3: Code Execution Phase
            CALL ExecuteCode(optimized_manim_code) → video_file
    
        STEP 4: Video Delivery
            DISPLAY video_file in Gradio interface
        
        OUTPUT: generated_video.mp4
    
    END Workflow
