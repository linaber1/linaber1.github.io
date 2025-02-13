## Welcome

Top k vs Top p sampling:
Let's say a language model is predicting the next word in the sentence:  

**"The sky is"**  

It generates probabilities for possible next words:  

| Word       | Probability |
|------------|------------|
| blue       | 0.50       |
| clear      | 0.20       |
| cloudy     | 0.15       |
| dark       | 0.10       |
| falling    | 0.05       |

### **Top-K Sampling (K = 3)**  
Only the **top 3** highest probability words are considered:  
- "blue" (0.50)  
- "clear" (0.20)  
- "cloudy" (0.15)  

The model then randomly picks one of these based on their probabilities, ignoring "dark" and "falling."  

### **Top-P Sampling (P = 0.85)**  
The model selects the smallest set of words whose total probability exceeds **0.85**:  
- "blue" (0.50)  
- "clear" (0.20)  
- "cloudy" (0.15)  
  _(Total = 0.85)_  

Again, it samples from this set. However, if probabilities were more spread out, the set would dynamically change.  

### **Key Difference**  
- **Top-K** always picks a fixed number (e.g., top 3 words).  
- **Top-P** selects words dynamically based on probability mass (e.g., enough words to exceed 0.85).  

Both methods help balance creativity and coherence in text generation! 🚀

<a href="index.html">Back to Home</a>

