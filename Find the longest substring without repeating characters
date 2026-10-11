function longestSubstring(str) {
    let seen = new Map();
    let left = 0;
    let maxLength = 0;

    for (let right = 0; right < str.length; right++) {
        let ch = str[right];

        if (seen.has(ch) && seen.get(ch) >= left) {
            left = seen.get(ch) + 1;
        }

        seen.set(ch, right);
        maxLength = Math.max(maxLength, right - left + 1);
    }

    return maxLength;
}

console.log(longestSubstring("abcabcbb"));
