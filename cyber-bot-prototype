import streamlit as st

# Custom CSS for "Hacker/Security" vibe
st.set_page_config(page_title="CyberCrime Prototype", page_icon="🛡️")
st.markdown("""
    <style>
    .main { background-color: #0e1117; color: #00ff41; font-family: 'Courier New', Courier, monospace; }
    stButton>button { background-color: #00ff41; color: black; font-weight: bold; }
    </style>
    """, unsafe_allow_html=True)

st.title("🛡️ Cyber Crime Detection Agent")
st.subheader("Prototype: Phishing & Social Engineering Analysis")

user_input = st.text_area("Paste suspicious Email, SMS, or Link here:", height=200)

if st.button("RUN SECURITY SCAN"):
    if user_input:
        with st.spinner('Analyzing patterns and metadata...'):
            # This is where your logic (or Gemini API) goes
            # For the prototype, we show a sample structured response:
            st.warning("⚠️ ANALYSIS COMPLETE")
            
            col1, col2 = st.columns(2)
            with col1:
                st.error("Risk Level: HIGH")
                st.info("Threat Type: Credential Harvesting")
            
            with col2:
                st.write("**Detected Red Flags:**")
                st.write("- Masked URL (bit.ly/...)")
                st.write("- High Urgency Language")
                st.write("- Sender domain spoofing")
            
            st.success("**Verdict:** This is a malicious phishing attempt. Do not click links or provide PII.")
    else:
        st.info("Please enter content to scan.")
